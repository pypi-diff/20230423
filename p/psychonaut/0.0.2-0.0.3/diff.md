# Comparing `tmp/psychonaut-0.0.2.tar.gz` & `tmp/psychonaut-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychonaut-0.0.2.tar", max compression
+gzip compressed data, was "psychonaut-0.0.3.tar", max compression
```

## Comparing `psychonaut-0.0.2.tar` & `psychonaut-0.0.3.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0     1069 2023-04-22 21:21:36.755778 psychonaut-0.0.2/LICENSE
--rw-r--r--   0        0        0     2325 2023-04-22 21:21:36.759778 psychonaut-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      469 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      721 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0      794 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      528 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/profile.py
--rw-r--r--   0        0        0      793 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      774 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/embed/external.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/embed/images.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/embed/record.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/defs.py
--rw-r--r--   0        0        0      875 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0     1007 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0      706 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0     1053 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0      784 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      455 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/like.py
--rw-r--r--   0        0        0      614 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/post.py
--rw-r--r--   0        0        0      463 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/repost.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      525 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/follow.py
--rw-r--r--   0        0        0      890 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0      872 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0      702 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      721 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0      894 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0      743 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/defs.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0      843 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      460 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0      876 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      460 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0      927 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      594 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      491 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0      845 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      891 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/label/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/label/defs.py
--rw-r--r--   0        0        0     1212 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0     1140 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0     1292 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1413 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/create_account.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/create_session.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/defs.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0      774 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0      788 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      815 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/get_session.py
--rw-r--r--   0        0        0      631 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      652 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      659 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      704 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0     1112 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      762 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      820 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      830 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0     1087 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0      730 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      625 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      523 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0     3017 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/session.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/cli/__init__.py
--rw-r--r--   0        0        0     1682 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/cli/cli.py
--rw-r--r--   0        0        0     1219 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/common_web/__init__.py
--rw-r--r--   0        0        0     2364 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/common_web/ipld.py
--rw-r--r--   0        0        0      421 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/common_web/ipld_test.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/__init__.py
--rw-r--r--   0        0        0     1347 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/did.py
--rw-r--r--   0        0        0     2106 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/did_test.py
--rw-r--r--   0        0        0     3117 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/handle.py
--rw-r--r--   0        0        0     6649 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/handle_test.py
--rw-r--r--   0        0        0    15049 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/reserved.py
--rw-r--r--   0        0        0      672 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/resolve.py
--rw-r--r--   0        0        0      467 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/resolve_test.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/lexicon/__init__.py
--rw-r--r--   0        0        0     2003 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/lexicon/blob_refs.py
--rw-r--r--   0        0        0     7958 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/lexicon/codegen.py
--rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/lexicon/codegen_test.py
--rw-r--r--   0        0        0      212 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/ctx.py
--rw-r--r--   0        0        0      767 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/defs.py
--rw-r--r--   0        0        0     6822 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/fields.py
--rw-r--r--   0        0        0     2921 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/fields_test.py
--rw-r--r--   0        0        0     1900 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/formats.py
--rw-r--r--   0        0        0     1919 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/formats_test.py
--rw-r--r--   0        0        0      939 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/tools.py
--rw-r--r--   0        0        0     8801 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/types.py
--rw-r--r--   0        0        0     3785 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/types_test.py
--rw-r--r--   0        0        0     1909 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/util.py
--rw-r--r--   0        0        0       23 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/nsid/__init__.py
--rw-r--r--   0        0        0     3003 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/nsid/nsid.py
--rw-r--r--   0        0        0     3287 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/nsid/nsid_test.py
--rw-r--r--   0        0        0     3716 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/uri/__init__.py
--rw-r--r--   0        0        0    17624 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/uri/uri_test.py
--rw-r--r--   0        0        0     3912 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/uri/validation.py
--rw-r--r--   0        0        0     1025 2023-04-22 21:21:36.779778 psychonaut-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 psychonaut-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-22 21:21:36.755778 psychonaut-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2516 2023-04-22 21:38:02.569876 psychonaut-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.3/psychonaut/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.3/psychonaut/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.3/psychonaut/api/lexicons/app/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      469 2023-04-22 21:21:36.767778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      721 2023-04-22 21:21:36.767778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0      794 2023-04-22 21:21:36.767778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      528 2023-04-22 21:21:36.767778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      793 2023-04-22 21:21:36.767778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      774 2023-04-22 21:21:36.767778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/embed/external.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/embed/images.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/embed/record.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0      875 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0     1007 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0      706 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0     1053 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0      784 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      455 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/like.py
+-rw-r--r--   0        0        0      614 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      463 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      525 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0      890 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0      872 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      702 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      721 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0      894 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0      743 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      843 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      460 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0      876 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      460 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0      927 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      594 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      491 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0      845 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      891 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/label/defs.py
+-rw-r--r--   0        0        0     1212 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0     1140 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0     1292 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1413 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/defs.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0      774 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0      788 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      815 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0      631 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      652 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      659 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      704 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0     1112 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      762 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      820 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      830 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0     1087 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0      730 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      625 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      523 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0     3017 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/api/session.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/cli/__init__.py
+-rw-r--r--   0        0        0     1704 2023-04-22 21:40:36.127373 psychonaut-0.0.3/psychonaut/cli/cli.py
+-rw-r--r--   0        0        0     1219 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/common_web/__init__.py
+-rw-r--r--   0        0        0     2364 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/common_web/ipld.py
+-rw-r--r--   0        0        0      421 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/common_web/ipld_test.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/identifier/__init__.py
+-rw-r--r--   0        0        0     1347 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/identifier/did.py
+-rw-r--r--   0        0        0     2106 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/identifier/did_test.py
+-rw-r--r--   0        0        0     3117 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/identifier/handle.py
+-rw-r--r--   0        0        0     6649 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/identifier/handle_test.py
+-rw-r--r--   0        0        0    15049 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/identifier/reserved.py
+-rw-r--r--   0        0        0      672 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/identifier/resolve.py
+-rw-r--r--   0        0        0      467 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/identifier/resolve_test.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/lexicon/__init__.py
+-rw-r--r--   0        0        0     2003 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/lexicon/blob_refs.py
+-rw-r--r--   0        0        0     7958 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/lexicon/codegen.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.3/psychonaut/lexicon/codegen_test.py
+-rw-r--r--   0        0        0      212 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/lexicon/ctx.py
+-rw-r--r--   0        0        0      767 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/lexicon/defs.py
+-rw-r--r--   0        0        0     6822 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/lexicon/fields.py
+-rw-r--r--   0        0        0     2921 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/lexicon/fields_test.py
+-rw-r--r--   0        0        0     1900 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/lexicon/formats.py
+-rw-r--r--   0        0        0     1919 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/lexicon/formats_test.py
+-rw-r--r--   0        0        0      939 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/lexicon/tools.py
+-rw-r--r--   0        0        0     8801 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/lexicon/types.py
+-rw-r--r--   0        0        0     3785 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/lexicon/types_test.py
+-rw-r--r--   0        0        0     1909 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/lexicon/util.py
+-rw-r--r--   0        0        0       23 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/nsid/__init__.py
+-rw-r--r--   0        0        0     3003 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/nsid/nsid.py
+-rw-r--r--   0        0        0     3287 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/nsid/nsid_test.py
+-rw-r--r--   0        0        0     3716 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/uri/__init__.py
+-rw-r--r--   0        0        0    17624 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/uri/uri_test.py
+-rw-r--r--   0        0        0     3912 2023-04-22 21:21:36.779778 psychonaut-0.0.3/psychonaut/uri/validation.py
+-rw-r--r--   0        0        0     1025 2023-04-22 21:41:22.438638 psychonaut-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3463 1970-01-01 00:00:00.000000 psychonaut-0.0.3/PKG-INFO
```

### Comparing `psychonaut-0.0.2/LICENSE` & `psychonaut-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/README.md` & `psychonaut-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 Almost certainly not. Right now it's a bucket of slop. I offer no 
 guarantees about the stability of the API, the correctness of the
 implementation, or the quality of the documentation. 
 
 If you want to use it, go ahead,
 
 ```bash
+# In your venv or mamba env or whatever
 pip install psychonaut
 ```
 
 to use it as a library. This also installs the `psychonaut` command line tool.
 
 ```bash
 psychonaut --help
@@ -44,15 +45,24 @@
 export BSKY_USERNAME=yourusername
 export BSKY_PASSWORD=yourpassword
 psychonaut poast "hey look, an annoying cron job"
 ```
 
 But definitely be mindful of the version because I'm going to break your code.
 
-todo: [pipx version](https://pypa.github.io/pipx/)
+Alternatively, just use [pipx](https://pypa.github.io/pipx/)
+
+```bash
+pipx install psychonaut
+
+export BSKY_USERNAME=yourusername
+export BSKY_PASSWORD=yourpassword
+
+psychonaut poast "hell yea, pipx"
+```
 
 # How is this made?
 
 This is a collaboration between the [atproto repo](https://github.com/bluesky-social/atproto),
 me, and my friend ChatGPT (using GPT-4). I've been toying around with this 
 automatic `langa`<->`langb` transpiler in [langchain](https://github.com/hwchase17/langchain).
 My original goal was to jointly build that while making my python client from the `atproto`
```

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/get_profiles.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/actor/get_profiles.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/get_suggestions.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/actor/get_suggestions.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/profile.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/actor/profile.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/search_actors.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/actor/search_actors.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/search_actors_typeahead.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/actor/search_actors_typeahead.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_author_feed.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/get_author_feed.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_likes.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/get_likes.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_post_thread.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/get_post_thread.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_reposted_by.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/get_reposted_by.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_timeline.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/get_timeline.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/post.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/feed/post.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/follow.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/graph/follow.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/get_followers.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/graph/get_followers.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/get_follows.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/graph/get_follows.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/get_mutes.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/graph/get_mutes.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/notification/get_unread_count.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/notification/get_unread_count.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/notification/list_notifications.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/notification/list_notifications.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/unspecced/get_popular.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/app/bsky/unspecced/get_popular.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_invite_codes.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/get_invite_codes.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_moderation_actions.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/get_moderation_actions.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_moderation_reports.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/get_moderation_reports.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_record.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/get_record.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/search_repos.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/admin/search_repos.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/identity/resolve_handle.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/identity/resolve_handle.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/label/query_labels.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/label/query_labels.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/describe_repo.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/repo/describe_repo.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/get_record.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/repo/get_record.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/list_records.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/repo/list_records.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/describe_server.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/describe_server.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/get_account_invite_codes.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/get_account_invite_codes.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/get_session.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/get_session.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/list_app_passwords.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/server/list_app_passwords.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_blob.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_blob.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_blocks.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_blocks.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_checkout.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_checkout.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_commit_path.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_commit_path.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_head.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_head.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_record.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_record.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_repo.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/get_repo.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/list_blobs.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/list_blobs.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/list_repos.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/list_repos.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/notify_of_update.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/notify_of_update.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/request_crawl.py` & `psychonaut-0.0.3/psychonaut/api/lexicons/com/atproto/sync/request_crawl.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/api/session.py` & `psychonaut-0.0.3/psychonaut/api/session.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/cli/cli.py` & `psychonaut-0.0.3/psychonaut/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 from datetime import datetime
 import os
 import sys
 from typing import List
 import click
 import asyncio
 from functools import wraps
-from psychonaut.api.lexicons.app.bsky.actor.get_profiles import GetProfilesReq, get_profiles as get_profiles_f
-from psychonaut.api.lexicons.com.atproto.identity.resolve_handle import ResolveHandleReq, resolve_handle as resolve_handle_f
+from psychonaut.api.lexicons.app.bsky.actor.get_profiles import (
+    GetProfilesReq,
+    get_profiles as get_profiles_f,
+)
+from psychonaut.api.lexicons.com.atproto.identity.resolve_handle import (
+    ResolveHandleReq,
+    resolve_handle as resolve_handle_f,
+)
 from psychonaut.client import get_simple_client_session
 from psychonaut.api.lexicons.app.bsky.feed.post import PostReq, post
 
 
 def as_async(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         return asyncio.run(func(*args, **kwargs))
+
     return wrapper
 
+
 @click.group()
 def cli():
     pass
 
 
 @cli.command()
 @click.argument("text")
 @as_async
 async def poast(text: str):
     async with get_simple_client_session() as sess:
         req = PostReq(text=text, createdAt=datetime.utcnow().isoformat())
         resp = await post(sess, req)
-        print(resp.json())
+        print(resp)
+
 
 @cli.command()
 @click.argument("handle")
 @as_async
 async def resolve_handle(handle: str):
     async with get_simple_client_session() as sess:
         req = ResolveHandleReq(handle=handle)
@@ -53,9 +62,9 @@
         req = GetProfilesReq(actors=actors)
         resp = await get_profiles_f(sess, req)
         for profile in resp.profiles:
             print(resp.json())
 
 
 # TODO: test poetry install
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `psychonaut-0.0.2/psychonaut/client/__init__.py` & `psychonaut-0.0.3/psychonaut/client/__init__.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/common_web/ipld.py` & `psychonaut-0.0.3/psychonaut/common_web/ipld.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/identifier/did.py` & `psychonaut-0.0.3/psychonaut/identifier/did.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/identifier/did_test.py` & `psychonaut-0.0.3/psychonaut/identifier/did_test.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/identifier/handle.py` & `psychonaut-0.0.3/psychonaut/identifier/handle.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/identifier/handle_test.py` & `psychonaut-0.0.3/psychonaut/identifier/handle_test.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/identifier/reserved.py` & `psychonaut-0.0.3/psychonaut/identifier/reserved.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/identifier/resolve.py` & `psychonaut-0.0.3/psychonaut/identifier/resolve.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/lexicon/blob_refs.py` & `psychonaut-0.0.3/psychonaut/lexicon/blob_refs.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/lexicon/codegen.py` & `psychonaut-0.0.3/psychonaut/lexicon/codegen.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/lexicon/defs.py` & `psychonaut-0.0.3/psychonaut/lexicon/defs.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/lexicon/fields.py` & `psychonaut-0.0.3/psychonaut/lexicon/fields.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/lexicon/fields_test.py` & `psychonaut-0.0.3/psychonaut/lexicon/fields_test.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/lexicon/formats.py` & `psychonaut-0.0.3/psychonaut/lexicon/formats.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/lexicon/formats_test.py` & `psychonaut-0.0.3/psychonaut/lexicon/formats_test.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/lexicon/tools.py` & `psychonaut-0.0.3/psychonaut/lexicon/tools.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/lexicon/types.py` & `psychonaut-0.0.3/psychonaut/lexicon/types.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/lexicon/types_test.py` & `psychonaut-0.0.3/psychonaut/lexicon/types_test.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/lexicon/util.py` & `psychonaut-0.0.3/psychonaut/lexicon/util.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/nsid/nsid.py` & `psychonaut-0.0.3/psychonaut/nsid/nsid.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/nsid/nsid_test.py` & `psychonaut-0.0.3/psychonaut/nsid/nsid_test.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/uri/__init__.py` & `psychonaut-0.0.3/psychonaut/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/uri/uri_test.py` & `psychonaut-0.0.3/psychonaut/uri/uri_test.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/psychonaut/uri/validation.py` & `psychonaut-0.0.3/psychonaut/uri/validation.py`

 * *Files identical despite different names*

### Comparing `psychonaut-0.0.2/pyproject.toml` & `psychonaut-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychonaut"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python async client and TUI for bsky"
 authors = ["generativist <jbn@abreka.com>"]
 readme = "README.md"
 homepage = "https://github.com/jbn/psychonaut"
 repository = "https://github.com/jbn/psychonaut"
 documentation = "https://github.com/jbn/psychonaut"
 license = "MIT"
```

### Comparing `psychonaut-0.0.2/PKG-INFO` & `psychonaut-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychonaut
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python async client and TUI for bsky
 Home-page: https://github.com/jbn/psychonaut
 License: MIT
 Author: generativist
 Author-email: jbn@abreka.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -53,14 +53,15 @@
 Almost certainly not. Right now it's a bucket of slop. I offer no 
 guarantees about the stability of the API, the correctness of the
 implementation, or the quality of the documentation. 
 
 If you want to use it, go ahead,
 
 ```bash
+# In your venv or mamba env or whatever
 pip install psychonaut
 ```
 
 to use it as a library. This also installs the `psychonaut` command line tool.
 
 ```bash
 psychonaut --help
@@ -69,15 +70,24 @@
 export BSKY_USERNAME=yourusername
 export BSKY_PASSWORD=yourpassword
 psychonaut poast "hey look, an annoying cron job"
 ```
 
 But definitely be mindful of the version because I'm going to break your code.
 
-todo: [pipx version](https://pypa.github.io/pipx/)
+Alternatively, just use [pipx](https://pypa.github.io/pipx/)
+
+```bash
+pipx install psychonaut
+
+export BSKY_USERNAME=yourusername
+export BSKY_PASSWORD=yourpassword
+
+psychonaut poast "hell yea, pipx"
+```
 
 # How is this made?
 
 This is a collaboration between the [atproto repo](https://github.com/bluesky-social/atproto),
 me, and my friend ChatGPT (using GPT-4). I've been toying around with this 
 automatic `langa`<->`langb` transpiler in [langchain](https://github.com/hwchase17/langchain).
 My original goal was to jointly build that while making my python client from the `atproto`
```

