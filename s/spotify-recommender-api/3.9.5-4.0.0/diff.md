# Comparing `tmp/spotify_recommender_api-3.9.5-py3-none-any.whl.zip` & `tmp/spotify_recommender_api-4.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 34131 bytes, number of entries: 12
--rw-rw-r--  2.0 unx       21 b- defN 23-Mar-24 10:44 spotify_recommender_api/__init__.py
--rw-rw-r--  2.0 unx      927 b- defN 23-Mar-04 17:44 spotify_recommender_api/authentication.py
--rw-rw-r--  2.0 unx    14242 b- defN 23-Mar-04 17:42 spotify_recommender_api/core.py
--rw-rw-r--  2.0 unx     1320 b- defN 23-Mar-04 17:41 spotify_recommender_api/error.py
--rw-rw-r--  2.0 unx    87641 b- defN 23-Mar-05 23:41 spotify_recommender_api/recommender.py
--rw-rw-r--  2.0 unx     4393 b- defN 23-Mar-04 17:44 spotify_recommender_api/request_handler.py
+Zip file size: 36886 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx       21 b- defN 23-Apr-22 18:23 spotify_recommender_api/__init__.py
+-rw-rw-r--  2.0 unx     1303 b- defN 23-Apr-22 18:20 spotify_recommender_api/authentication.py
+-rw-rw-r--  2.0 unx    14242 b- defN 23-Apr-22 18:22 spotify_recommender_api/core.py
+-rw-rw-r--  2.0 unx     1966 b- defN 23-Apr-22 18:22 spotify_recommender_api/error.py
+-rw-rw-r--  2.0 unx    91849 b- defN 23-Apr-22 18:22 spotify_recommender_api/recommender.py
+-rw-rw-r--  2.0 unx     5866 b- defN 23-Apr-22 18:22 spotify_recommender_api/request_handler.py
 -rw-rw-r--  2.0 unx       99 b- defN 22-Jun-25 22:21 spotify_recommender_api/sensitive.py
--rw-rw-r--  2.0 unx     9124 b- defN 23-Mar-04 17:43 spotify_recommender_api/util.py
--rw-rw-r--  2.0 unx    20775 b- defN 23-Mar-24 10:45 spotify_recommender_api-3.9.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-24 10:45 spotify_recommender_api-3.9.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       24 b- defN 23-Mar-24 10:45 spotify_recommender_api-3.9.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1102 b- defN 23-Mar-24 10:45 spotify_recommender_api-3.9.5.dist-info/RECORD
-12 files, 139760 bytes uncompressed, 32241 bytes compressed:  76.9%
+-rw-rw-r--  2.0 unx     6637 b- defN 23-Apr-22 18:24 spotify_recommender_api/server.py
+-rw-rw-r--  2.0 unx     9111 b- defN 23-Apr-22 18:22 spotify_recommender_api/util.py
+-rw-rw-r--  2.0 unx    20821 b- defN 23-Apr-22 18:56 spotify_recommender_api-4.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-22 18:56 spotify_recommender_api-4.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       24 b- defN 23-Apr-22 18:56 spotify_recommender_api-4.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1193 b- defN 23-Apr-22 18:56 spotify_recommender_api-4.0.0.dist-info/RECORD
+13 files, 153224 bytes uncompressed, 34854 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -15,23 +15,26 @@
 
 Filename: spotify_recommender_api/request_handler.py
 Comment: 
 
 Filename: spotify_recommender_api/sensitive.py
 Comment: 
 
+Filename: spotify_recommender_api/server.py
+Comment: 
+
 Filename: spotify_recommender_api/util.py
 Comment: 
 
-Filename: spotify_recommender_api-3.9.5.dist-info/METADATA
+Filename: spotify_recommender_api-4.0.0.dist-info/METADATA
 Comment: 
 
-Filename: spotify_recommender_api-3.9.5.dist-info/WHEEL
+Filename: spotify_recommender_api-4.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: spotify_recommender_api-3.9.5.dist-info/top_level.txt
+Filename: spotify_recommender_api-4.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: spotify_recommender_api-3.9.5.dist-info/RECORD
+Filename: spotify_recommender_api-4.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spotify_recommender_api/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '3.9.5'
+__version__ = '4.0.0'
```

## spotify_recommender_api/authentication.py

```diff
@@ -1,15 +1,50 @@
-import webbrowser
+import os
+from spotify_recommender_api.sensitive import *
+from spotify_recommender_api.server import up_server
+from spotify_recommender_api.request_handler import post_request_with_auth
 
-def get_auth():
-    print('In order to get the authentication code that allows everything to work nicely, you have to get to the spotify console and set the OAuth token scopes (powers) as follow, then you click onto the token then ctrl + A, to select it all, then crtl + C to copy it, then provide it to the class constructor and its all set\n')
-    scope = 'playlist-modify-private playlist-read-private user-library-read user-library-modify user-top-read\n'
-
-    print(scope)
-    answer = input("Ready to be redirected to get the token (y/n)? ")
-    while answer.lower() not in ['y', 'n']:
-        answer = input("Please select a valid response about being redirected to get the token: ")
-    if answer.lower() == 'y':
-        webbrowser.open('https://developer.spotify.com/console/get-artist/')
-    else:
-        print('In order to get the token and use this lib, it is necessary to get the auth token')
 
+def get_auth() -> str:
+    """Function to retrieve the authentication token for the first time in the execution
+
+    Returns:
+        str: Auth Token
+    """
+    up_server()
+
+    with open('./.spotify-recommender-util/execution.txt', 'r') as f:
+        auth_token = f.readline()
+
+    if os.path.exists("./.spotify-recommender-util/execution-status.txt"):
+        os.remove("./.spotify-recommender-util/execution-status.txt")
+
+    return auth_token
+
+
+def refresh_token() -> str:
+    """Function to refresh the auth token
+
+    Returns:
+        str: Refreshed auth token
+    """
+
+    print('Retrieving refresh token')
+
+    with open('./.spotify-recommender-util/execution.txt', 'r') as f:
+        refresh_token = f.readline()
+
+    req = post_request_with_auth(
+        url="https://accounts.spotify.com/api/token",
+        auth=(CLIENT_ID, CLIENT_SECRET),
+        data={
+            'grant_type': 'refresh_token',
+            'refresh_token': refresh_token
+        }
+    )
+
+    token = req['access_token']
+
+    with open('./.spotify-recommender-util/execution.txt', 'w') as f:
+        f.write(token)
+
+    return token
```

## spotify_recommender_api/error.py

```diff
@@ -1,7 +1,9 @@
+from typing import Callable
+
 class HTTPRequestError(Exception):
     """Generic exception for HTTP Request Exceptions
         It can receive the error code and function name, and the function arguments, besides the message, to better help debugging the error
     """
     def __init__(
         self,
         message=None,
@@ -26,8 +28,22 @@
         super().__init__(f'{message}{err_code}')
 
 class TooManyRequestsError(HTTPRequestError):
     """Generic exception for HTTP Request Exceptions
         It can receive the function name and the function arguments, besides the message, to better help debugging the error
     """
     def __init__(self, func_name=None, message=None, *args, **kwargs):
-        super().__init__(err_code='429 Too Many Requests', func_name=func_name, message=message, *args, **kwargs)
+        super().__init__(err_code='429 Too Many Requests', func_name=func_name, message=message, *args, **kwargs)
+
+class AccessTokenExpiredError(HTTPRequestError):
+    """Exception raised when the SpofifyAPI access token has expired
+        It can receive the function name and the function arguments, besides the message, to better help debugging the error
+    """
+    func: Callable
+    args: list
+    kwargs: 'dict[str,]'
+
+    def __init__(self, func_name: str = None, func: Callable = None, message: str = None, *args, **kwargs):
+        super().__init__(err_code='401 Access Token Expired', func_name=func_name, message=message, *args, **kwargs)
+        self.func = func
+        self.args = args
+        self.kwargs = kwargs
```

## spotify_recommender_api/recommender.py

```diff
@@ -1,17 +1,18 @@
 import os
 import re
 import operator
 import pandas as pd
 import spotify_recommender_api.util as util
 import spotify_recommender_api.core as core
+import spotify_recommender_api.authentication as auth
 import spotify_recommender_api.request_handler as requests
 from functools import reduce
 from spotify_recommender_api.sensitive import *
-from spotify_recommender_api.authentication import get_auth
+from spotify_recommender_api.error import AccessTokenExpiredError
 
 
 pd.options.mode.chained_assignment = None
 
 
 class SpotifyAPI:
     """
@@ -110,18 +111,20 @@
 
         # Note
         Ran automatically but can last as long as 2.5 seconds for each song (can be worse depending on the network connection) inside of the playlist, not because it is compute demanding but because it needs to do a up to a handful of http requests per song, which can take a while
 
         """
         self.__all_genres = []
         try:
-            for offset in range(0, util.get_total_song_count(playlist_id=self.__playlist_id, headers=self.__headers), 100):
+            total_song_count = util.get_total_song_count(playlist_id=self.__playlist_id, headers=self.__headers)
+            for offset in range(0, total_song_count, 100):
+                print(f'Songs mapped: {offset}/{total_song_count}')
                 all_genres_res = requests.get_request(
                     headers=self.__headers,
-                    url=f'https://api.spotify.com/v1/playlists/{self.__playlist_id}/tracks?limit=100&{offset=}'
+                    url=f'https://api.spotify.com/v1/playlists/{self.__playlist_id}/tracks?limit=100&{offset=!s}'
                 )
                 for song in all_genres_res.json()["items"]:
                     (id, name, popularity, artist, added_at), song_genres = util.song_data(
                         song=song), self.__get_song_genres(song)
                     song['id'] = id
                     danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
                         song=song, headers=self.__headers)
@@ -212,20 +215,23 @@
         else:
             if not playlist_url:
                 raise ValueError(
                     'Either the playlist url or its id must be specified')
             self.__playlist_id = util.playlist_url_to_id(url=playlist_url)
             self.__playlist_url = playlist_url
 
-        self.__base_playlist_name = util.get_base_playlist_name(
-            playlist_id=self.__playlist_id, headers=self.__headers)
+        self.__base_playlist_name = util.get_base_playlist_name(playlist_id=self.__playlist_id, headers=self.__headers)
+
+        print('Mapping playlist items')
 
         if self.__get_playlist():
             self.__get_playlist_items()
 
+        print('Seting up some operations with the playlist')
+
         self.__playlist_adjustments()
 
         self.__song_dict = core.knn_prepared_data(playlist=self.__playlist)
         self.__prepare_favorites_playlist()
 
         if self.__update_created_files:
             self.playlist_to_csv()
@@ -466,33 +472,48 @@
         """
         try:
             if not (1 < K <= 1500):
                 raise ValueError(
                     f'Value for K must be between 1 and 1500 on creation of recommendation for the song {song}')
 
             self.__song_name = song
-            df = self.__get_recommendations('song', song, K)
-            playlist_name = f'{song} Related'
 
-            if print_base_caracteristics:
-                index = self.__get_index_for_song(song)
-                caracteristics = self.__song_dict[index]
-                name, genres, artists, popularity, _, danceability, energy, instrumentalness, tempo, valence = list(
-                    caracteristics.values())[1:11]
-                util.print_base_caracteristics(
-                    name, genres, artists, popularity, danceability, energy, instrumentalness, tempo, valence)
+            for _ in range(2):
+                try:
+
+                    df = self.__get_recommendations('song', song, K)
+                    playlist_name = f'{song} Related'
+
+                    if print_base_caracteristics:
+                        index = self.__get_index_for_song(song)
+                        caracteristics = self.__song_dict[index]
+                        name, genres, artists, popularity, _, danceability, energy, instrumentalness, tempo, valence = list(
+                            caracteristics.values())[1:11]
+                        util.print_base_caracteristics(
+                            name, genres, artists, popularity, danceability, energy, instrumentalness, tempo, valence)
+
+                    if generate_csv:
+                        df.to_csv(f'{playlist_name}.csv')
 
-            if generate_csv:
-                df.to_csv(f'{playlist_name}.csv')
+                    if generate_parquet:
+                        df.to_parquet(f'{playlist_name}.parquet', compression='snappy')
 
-            if generate_parquet:
-                df.to_parquet(f'{playlist_name}.parquet', compression='snappy')
+                    if build_playlist:
+                        self.__write_playlist('song', K, additional_info=song)
 
-            if build_playlist:
-                self.__write_playlist('song', K, additional_info=song)
+
+                except AccessTokenExpiredError as e:
+                    print('Error due to the access token expiration')
+                    auth_token = auth.refresh_token()
+
+                    self.__auth_token = auth_token
+
+                    self.__headers['Authorization'] = f'Bearer {auth_token}'
+                else:
+                    break
 
             return df if with_distance else df.drop(columns=['distance'])
 
         except ValueError as e:
             print(e)
 
     def __get_desired_dict_fields(self, index: int, song_dict: list = None) -> 'list[str]':
@@ -742,15 +763,15 @@
         """Function that returns the playlist as pandas DataFrame with the needed, human readable, columns
 
         Returns:
             pd.DataFrame: Playlist DataFrame
         """
         return self.__playlist[['id', 'name', 'artists', 'genres', 'popularity', 'added_at', 'danceability', 'energy', 'instrumentalness', 'tempo', 'valence']]
 
-    # @util.deprecated
+    @util.deprecated
     def get_short_term_favorites_playlist(
         self,
         generate_csv: bool = False,
         with_distance: bool = False,
         build_playlist: bool = False,
         generate_parquet: bool = False,
     ) -> pd.DataFrame:
@@ -780,15 +801,15 @@
             df.to_parquet(f'{playlist_name}.parquet', compression='snappy')
 
         if build_playlist:
             self.__write_playlist('short', 51)
 
         return df if with_distance else df.drop(columns=['distance'])
 
-    # @util.deprecated
+    @util.deprecated
     def get_medium_term_favorites_playlist(self, with_distance: bool = False, generate_csv: bool = False, generate_parquet: bool = False, build_playlist: bool = False) -> pd.DataFrame:
         """###DEPRECATED METHOD###\n
         Playlist which centralises the actions for a recommendation made for top 5 songs medium term
 
         Note
             The build_playlist option when set to True will change the user's library
 
@@ -815,14 +836,15 @@
             self.__write_playlist('medium', 51)
 
         return df if with_distance else df.drop(columns=['distance'])
 
     def __prepare_favorites_playlist(self):
         """###DEPRECATED METHOD###\n
         Note: Although this method and the whole medium and short term favorite category is deprecated, this method will stil run, since somebody may want to use it. Having that said, I do not recommend it
+
         Automatic creation of both the favorites related recommendations
         """
         try:
             self.__short_fav = self.__get_recommendations(
                 'short',  self.__end_prepared_fav_data('short'))
             self.__medium_fav = self.__get_recommendations(
                 'medium',  self.__end_prepared_fav_data('medium'))
@@ -848,23 +870,36 @@
             raise ValueError(
                 'time_range must be long, medium or short')
 
         if not (1 < K <= 1500):
             raise ValueError(
                 f'Value for K must be between 1 and 1500: {time_range} term most listened')
 
-        top = requests.get_request(
-            url=f'https://api.spotify.com/v1/me/top/tracks?{time_range=!s}_term&limit={K}', headers=self.__headers).json()
+        for _ in range(2):
+            try:
+
+                top = requests.get_request(
+                    url=f'https://api.spotify.com/v1/me/top/tracks?{time_range=!s}_term&limit={K}', headers=self.__headers).json()
 
-        top_songs = list(map(lambda song: {'id': song['id'], 'name': song['name'], 'genres': self.__get_song_genres(song), 'artists': list(map(
-            lambda artist: artist['name'], song['artists'])), 'popularity': song['popularity']}, top['items']))
+                top_songs = list(map(lambda song: {'id': song['id'], 'name': song['name'], 'genres': self.__get_song_genres(song), 'artists': list(map(
+                    lambda artist: artist['name'], song['artists'])), 'popularity': song['popularity']}, top['items']))
 
-        if build_playlist:
-            self.__write_playlist(
-                f'most-listened-{time_range}', K, additional_info=list(map(lambda x: x['id'], top_songs)))
+                if build_playlist:
+                    self.__write_playlist(
+                        f'most-listened-{time_range}', K, additional_info=list(map(lambda x: x['id'], top_songs)))
+
+            except AccessTokenExpiredError as e:
+                print('Error due to the access token expiration')
+                auth_token = auth.refresh_token()
+
+                self.__auth_token = auth_token
+
+                self.__headers['Authorization'] = f'Bearer {auth_token}'
+            else:
+                break
 
         return pd.DataFrame(data=list(map(lambda x: {'name': x['name'], 'genres': x['genres'], 'artists': x['artists'], 'popularity': x['popularity']}, top_songs)), columns=['name', 'artists', 'genres', 'popularity'])
 
     def update_all_generated_playlists(self, K: int = None):
         """Update all package generated playlists in batch
 
         Note:
@@ -1130,27 +1165,27 @@
                 song_dict = list(map(lambda x: {'id': x['id'], 'name': x['name'], 'artists': x['artists'], 'genres': x['genres'], 'artists_indexed': x['artists_indexed'], 'genres_indexed': x['genres_indexed'], 'popularity': x['popularity'], 'added_at': x['added_at'],
                                  'danceability': x['danceability'], 'energy': x['energy'], 'instrumentalness': x['instrumentalness'], 'tempo': x['tempo'], 'valence': x['valence']}, list(filter(lambda x: artist_name not in x['artists'], self.__song_dict))))
                 song_dict.append(artist_songs_record)
 
                 mix_songs = self.__get_recommendations(
                     'artist-related', song_dict, K=K-len(artist_songs))
 
-                ids = artist_songs['id'].append(mix_songs['id'])
+                ids = pd.concat([artist_songs['id'], mix_songs['id']])
 
                 if with_distance:
                     df = artist_songs[columns]
 
                     columns.append('distance')
 
                     df['distance'] = pd.to_numeric(0)
 
-                    df = df[columns].append(mix_songs[columns])
+                    df = pd.concat([df[columns], mix_songs[columns]])
 
                 else:
-                    df = artist_songs[columns].append(mix_songs[columns])
+                    df = pd.concat([artist_songs[columns], mix_songs[columns]])
 
                 if print_base_caracteristics and not _auto:
                     name = artist_songs_record['name']
                     genres = artist_songs_record['genres']
                     artists = artist_songs_record['artists']
                     popularity = artist_songs_record['popularity']
                     danceability = artist_songs_record['danceability']
@@ -1208,23 +1243,20 @@
 
         df_danceability = df.sort_values('danceability', ascending=True)
         df_energy = df.sort_values('energy', ascending=True)
         df_instrumentalness = df.sort_values(
             'instrumentalness', ascending=True)
         df_tempo = df.sort_values('tempo', ascending=True)
         df_valence = df.sort_values('valence', ascending=True)
-        mean_danceability = df['danceability'].mean()
         max_danceability = df_danceability.tail(n=1).reset_index(drop=True)
         min_danceability = df_danceability.head(n=1).reset_index(drop=True)
         max_energy = df_energy.tail(n=1).reset_index(drop=True)
         min_energy = df_energy.head(n=1).reset_index(drop=True)
-        max_instrumentalness = df_instrumentalness.tail(
-            n=1).reset_index(drop=True)
-        min_instrumentalness = df_instrumentalness.head(
-            n=1).reset_index(drop=True)
+        max_instrumentalness = df_instrumentalness.tail(n=1).reset_index(drop=True)
+        min_instrumentalness = df_instrumentalness.head(n=1).reset_index(drop=True)
         max_tempo = df_tempo.tail(n=1).reset_index(drop=True)
         min_tempo = df_tempo.head(n=1).reset_index(drop=True)
         max_valence = df_valence.tail(n=1).reset_index(drop=True)
         min_valence = df_valence.head(n=1).reset_index(drop=True)
 
         return {
             'max_danceability': {
@@ -1355,16 +1387,18 @@
                 'energy': min_valence['energy'][0],
                 'instrumentalness': min_valence['instrumentalness'][0],
                 'tempo': min_valence['tempo'][0],
                 'valence': min_valence['valence'][0]
             },
         }
 
+    @util.deprecated
     def refresh_token(self, token: str):
-        """Refreshes the authorization token for the Spotify API, so that it is not necessary to rerun the entire script using the package to reauthenticate
+        """###DEPRECATED METHOD###
+        Refreshes the authorization token for the Spotify API, so that it is not necessary to rerun the entire script using the package to reauthenticate
 
         Args:
             token (str): Token generated from the Spotify API Console, with the following scopes:
              - user-top-read
              - playlist-library-read
              - playlist-read-private
              - playlist-library-modify
@@ -1431,90 +1465,103 @@
         if not (1 < K <= 100):
             raise ValueError('K must be between 1 and 100')
 
         if main_criteria not in ['mixed', 'artists', 'tracks', 'genres']:
             raise ValueError(
                 "main_criteria must be one of the following: 'mixed', 'artists', 'tracks', 'genres'")
 
-        if main_criteria != 'tracks':
-            if self.__top_genres or self.__top_artists:
-                genres = self.__top_genres
-                artists = self.__top_artists
-
-            else:
-                top_artists_req = requests.get_request(
-                    url='https://api.spotify.com/v1/me/top/artists?time_range=short_term&limit=5', headers=self.__headers).json()['items']
+        for _ in range(2):
+            try:
 
-                artists = list(map(lambda x: x['id'], top_artists_req))
-                genres = list(set(reduce(
-                    lambda x, y: x + y, list(map(lambda x: x['genres'], top_artists_req)), [])))[:5]
-                self.__top_genres = genres
-                self.__top_artists = artists
-        if main_criteria not in ['artists']:
-            if self.__top_tracks:
-                tracks = self.__top_tracks
+                if main_criteria != 'tracks':
+                    if self.__top_genres or self.__top_artists:
+                        genres = self.__top_genres
+                        artists = self.__top_artists
+
+                    else:
+                        top_artists_req = requests.get_request(
+                            url='https://api.spotify.com/v1/me/top/artists?time_range=short_term&limit=5', headers=self.__headers).json()['items']
+
+                        artists = list(map(lambda x: x['id'], top_artists_req))
+                        genres = list(set(reduce(
+                            lambda x, y: x + y, list(map(lambda x: x['genres'], top_artists_req)), [])))[:5]
+                        self.__top_genres = genres
+                        self.__top_artists = artists
+                if main_criteria not in ['artists']:
+                    if self.__top_tracks:
+                        tracks = self.__top_tracks
+
+                    else:
+                        tracks = list(map(lambda x: x['id'], requests.get_request(
+                            url='https://api.spotify.com/v1/me/top/tracks?time_range=short_term&limit=5', headers=self.__headers).json()['items']))
+
+                        self.__top_tracks = tracks
+                url = f'https://api.spotify.com/v1/recommendations?limit={K}'
+
+                if main_criteria == 'artists':
+                    url += f'&seed_artists={",".join(artists)}'
+                elif main_criteria == 'genres':
+                    url += f'&seed_genres={",".join(genres[:4])}&seed_tracks={",".join(tracks[:1])}'
+                elif main_criteria == 'mixed':
+                    url += f'&seed_tracks={",".join(tracks[:2])}&seed_artists={",".join(artists[:1])}&seed_genres={",".join(genres[:2])}'
+                elif main_criteria == 'tracks':
+                    url += f'&seed_tracks={",".join(tracks)}'
 
-            else:
-                tracks = list(map(lambda x: x['id'], requests.get_request(
-                    url='https://api.spotify.com/v1/me/top/tracks?time_range=short_term&limit=5', headers=self.__headers).json()['items']))
+                recommendations = requests.get_request(
+                    url=url, headers=self.__headers).json()
 
-                self.__top_tracks = tracks
-        url = f'https://api.spotify.com/v1/recommendations?limit={K}'
+                if not recommendations.get("tracks"):
+                    print(
+                        f'There was a problem creating the profile recommendations based on {main_criteria}')
+                    return
 
-        if main_criteria == 'artists':
-            url += f'&seed_artists={",".join(artists)}'
-        elif main_criteria == 'genres':
-            url += f'&seed_genres={",".join(genres[:4])}&seed_tracks={",".join(tracks[:1])}'
-        elif main_criteria == 'mixed':
-            url += f'&seed_tracks={",".join(tracks[:2])}&seed_artists={",".join(artists[:1])}&seed_genres={",".join(genres[:2])}'
-        elif main_criteria == 'tracks':
-            url += f'&seed_tracks={",".join(tracks)}'
+                songs = []
 
-        recommendations = requests.get_request(
-            url=url, headers=self.__headers).json()
+                for song in recommendations["tracks"]:
+                    (id, name, popularity, artist), song_genres = util.song_data(
+                        song=song, added_at=False), self.__get_song_genres(song)
+                    song['id'] = id
+                    danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
+                        song=song, headers=self.__headers)
+                    songs.append({
+                        "id": id,
+                        "name": name,
+                        "artists": artist,
+                        "popularity": popularity,
+                        "genres": song_genres,
+                        "danceability": danceability,
+                        "energy": energy,
+                        "instrumentalness": instrumentalness,
+                        "tempo": tempo,
+                        "valence": valence
+                    })
 
-        if not recommendations.get("tracks"):
-            print(
-                f'There was a problem creating the profile recommendations based on {main_criteria}')
-            return
+                recommendations_playlist = pd.DataFrame(data=songs)
 
-        songs = []
+                ids = recommendations_playlist['id'].tolist()
 
-        for song in recommendations["tracks"]:
-            (id, name, popularity, artist), song_genres = util.song_data(
-                song=song, added_at=False), self.__get_song_genres(song)
-            song['id'] = id
-            danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
-                song=song, headers=self.__headers)
-            songs.append({
-                "id": id,
-                "name": name,
-                "artists": artist,
-                "popularity": popularity,
-                "genres": song_genres,
-                "danceability": danceability,
-                "energy": energy,
-                "instrumentalness": instrumentalness,
-                "tempo": tempo,
-                "valence": valence
-            })
+                if build_playlist:
+                    self.__profile_recommendation_date = save_with_date
+                    self.__profile_recommendation_criteria = main_criteria
 
-        recommendations_playlist = pd.DataFrame(data=songs)
+                    self.__write_playlist(
+                        K=K,
+                        type='profile-recommendation',
+                        additional_info=ids
+                    )
 
-        ids = recommendations_playlist['id'].tolist()
+            except AccessTokenExpiredError as e:
+                print('Error due to the access token expiration')
+                auth_token = auth.refresh_token()
 
-        if build_playlist:
-            self.__profile_recommendation_date = save_with_date
-            self.__profile_recommendation_criteria = main_criteria
+                self.__auth_token = auth_token
 
-            self.__write_playlist(
-                K=K,
-                type='profile-recommendation',
-                additional_info=ids
-            )
+                self.__headers['Authorization'] = f'Bearer {auth_token}'
+            else:
+                break
 
         return recommendations_playlist
 
     def get_playlist_recommendation(
         self,
         K: int = 50,
         time_range: str = 'all_time',
@@ -1542,102 +1589,115 @@
         if not (1 < K <= 100):
             raise ValueError('K must be between 1 and 100')
 
         if main_criteria not in ['mixed', 'artists', 'tracks', 'genres']:
             raise ValueError(
                 "main_criteria must be one of the following: 'mixed', 'artists', 'tracks', 'genres'")
 
-        audio_statistics = self.audio_features_statistics()
-
-        if main_criteria not in ['genres', 'tracks']:
-            top_artists_names = self.get_playlist_trending_artists(time_range=time_range)[
-                'name'][1:6].tolist()
-            artists = list(map(lambda x: requests.get_request(
-                url=f'https://api.spotify.com/v1/search?q={x}&type=artist&limit=1', headers=self.__headers).json()['artists']['items'][0]['id'], top_artists_names))
-
-        if main_criteria not in ['artists']:
-            if self.__top_tracks:
-                tracks = self.__top_tracks
 
-            else:
-                tracks = list(map(lambda x: x['id'], requests.get_request(
-                    url='https://api.spotify.com/v1/me/top/tracks?time_range=short_term&limit=5', headers=self.__headers).json()['items']))
+        for _ in range(2):
+            try:
+                audio_statistics = self.audio_features_statistics()
 
-                self.__top_tracks = tracks
-        if main_criteria != 'artists':
-            genres = self.get_playlist_trending_genres(time_range=time_range)[
-                'name'][1:6].tolist()[:5]
-
-        min_tempo = audio_statistics['min_tempo'] * 0.8
-        max_tempo = audio_statistics['max_tempo'] * 1.2
-        target_tempo = audio_statistics['mean_tempo']
-        min_energy = audio_statistics['min_energy'] * 0.8
-        max_energy = audio_statistics['max_energy'] * 1.2
-        target_energy = audio_statistics['mean_energy']
-        min_valence = audio_statistics['min_valence'] * 0.8
-        max_valence = audio_statistics['max_valence'] * 1.2
-        target_valence = audio_statistics['mean_valence']
-        min_danceability = audio_statistics['min_danceability'] * 0.8
-        max_danceability = audio_statistics['max_danceability'] * 1.2
-        target_danceability = audio_statistics['mean_danceability']
-        min_instrumentalness = audio_statistics['min_instrumentalness'] * 0.8
-        max_instrumentalness = audio_statistics['max_instrumentalness'] * 1.2
-        target_instrumentalness = audio_statistics['mean_instrumentalness']
+                if main_criteria not in ['genres', 'tracks']:
+                    top_artists_names = self.get_playlist_trending_artists(time_range=time_range)[
+                        'name'][1:6].tolist()
+                    artists = list(map(lambda x: requests.get_request(
+                        url=f'https://api.spotify.com/v1/search?q={x}&type=artist&limit=1', headers=self.__headers).json()['artists']['items'][0]['id'], top_artists_names))
+
+                if main_criteria not in ['artists']:
+                    if self.__top_tracks:
+                        tracks = self.__top_tracks
+
+                    else:
+                        tracks = list(map(lambda x: x['id'], requests.get_request(
+                            url='https://api.spotify.com/v1/me/top/tracks?time_range=short_term&limit=5', headers=self.__headers).json()['items']))
+
+                        self.__top_tracks = tracks
+                if main_criteria != 'artists':
+                    genres = self.get_playlist_trending_genres(time_range=time_range)[
+                        'name'][1:6].tolist()[:5]
+
+                min_tempo = audio_statistics['min_tempo'] * 0.8
+                max_tempo = audio_statistics['max_tempo'] * 1.2
+                target_tempo = audio_statistics['mean_tempo']
+                min_energy = audio_statistics['min_energy'] * 0.8
+                max_energy = audio_statistics['max_energy'] * 1.2
+                target_energy = audio_statistics['mean_energy']
+                min_valence = audio_statistics['min_valence'] * 0.8
+                max_valence = audio_statistics['max_valence'] * 1.2
+                target_valence = audio_statistics['mean_valence']
+                min_danceability = audio_statistics['min_danceability'] * 0.8
+                max_danceability = audio_statistics['max_danceability'] * 1.2
+                target_danceability = audio_statistics['mean_danceability']
+                min_instrumentalness = audio_statistics['min_instrumentalness'] * 0.8
+                max_instrumentalness = audio_statistics['max_instrumentalness'] * 1.2
+                target_instrumentalness = audio_statistics['mean_instrumentalness']
+
+                url = f'https://api.spotify.com/v1/recommendations?limit={K}'
+
+                if main_criteria == 'artists':
+                    url += f'&seed_artists={",".join(artists)}'
+
+                elif main_criteria == 'genres':
+                    url += f'&seed_genres={",".join(genres[:4])}&seed_tracks={",".join(tracks[:1])}'
+                elif main_criteria == 'mixed':
+                    url += f'&seed_tracks={",".join(tracks[:1])}&seed_artists={",".join(artists[:2])}&seed_genres={",".join(genres[:2])}'
+                elif main_criteria == 'tracks':
+                    url += f'&seed_tracks={",".join(tracks[:2])}&seed_genres={",".join(genres[:3])}'
+                url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
+
+                recommendations = requests.get_request(
+                    url=url, headers=self.__headers).json()
+
+                songs = []
+
+                for song in recommendations["tracks"]:
+                    (id, name, popularity, artist), song_genres = util.song_data(
+                        song=song, added_at=False), self.__get_song_genres(song)
+                    song['id'] = id
+                    danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
+                        song=song, headers=self.__headers)
+                    songs.append({
+                        "id": id,
+                        "name": name,
+                        "artists": artist,
+                        "popularity": popularity,
+                        "genres": song_genres,
+                        "danceability": danceability,
+                        "energy": energy,
+                        "instrumentalness": instrumentalness,
+                        "tempo": tempo,
+                        "valence": valence
+                    })
 
-        url = f'https://api.spotify.com/v1/recommendations?limit={K}'
+                recommendations_playlist = pd.DataFrame(data=songs)
 
-        if main_criteria == 'artists':
-            url += f'&seed_artists={",".join(artists)}'
+                ids = recommendations_playlist['id'].tolist()
 
-        elif main_criteria == 'genres':
-            url += f'&seed_genres={",".join(genres[:4])}&seed_tracks={",".join(tracks[:1])}'
-        elif main_criteria == 'mixed':
-            url += f'&seed_tracks={",".join(tracks[:1])}&seed_artists={",".join(artists[:2])}&seed_genres={",".join(genres[:2])}'
-        elif main_criteria == 'tracks':
-            url += f'&seed_tracks={",".join(tracks[:2])}&seed_genres={",".join(genres[:3])}'
-        url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
-
-        recommendations = requests.get_request(
-            url=url, headers=self.__headers).json()
-
-        songs = []
-
-        for song in recommendations["tracks"]:
-            (id, name, popularity, artist), song_genres = util.song_data(
-                song=song, added_at=False), self.__get_song_genres(song)
-            song['id'] = id
-            danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
-                song=song, headers=self.__headers)
-            songs.append({
-                "id": id,
-                "name": name,
-                "artists": artist,
-                "popularity": popularity,
-                "genres": song_genres,
-                "danceability": danceability,
-                "energy": energy,
-                "instrumentalness": instrumentalness,
-                "tempo": tempo,
-                "valence": valence
-            })
+                if build_playlist:
+                    self.__playlist_recommendation_date = save_with_date
+                    self.__playlist_recommendation_time_range = time_range
+                    self.__playlist_recommendation_criteria = main_criteria
 
-        recommendations_playlist = pd.DataFrame(data=songs)
+                    self.__write_playlist(
+                        K=K,
+                        type='playlist-recommendation',
+                        additional_info=ids
+                    )
 
-        ids = recommendations_playlist['id'].tolist()
+            except AccessTokenExpiredError as e:
+                print('Error due to the access token expiration')
+                auth_token = auth.refresh_token()
 
-        if build_playlist:
-            self.__playlist_recommendation_date = save_with_date
-            self.__playlist_recommendation_time_range = time_range
-            self.__playlist_recommendation_criteria = main_criteria
+                self.__auth_token = auth_token
 
-            self.__write_playlist(
-                K=K,
-                type='playlist-recommendation',
-                additional_info=ids
-            )
+                self.__headers['Authorization'] = f'Bearer {auth_token}'
+            else:
+                break
 
         return recommendations_playlist
 
     def get_general_recommendation(
         self,
         K: int = 50,
         genres_info: 'list[str]' = [],
@@ -1680,152 +1740,164 @@
 
         url = f'https://api.spotify.com/v1/recommendations?limit={K}'
 
         description = 'General Recommendation based on '
 
         types = []
 
-        if artists_info:
-            types.append('artists')
-            description += 'the artists '
-            for artist in artists_info:
-                description += f'{artist}, '
-
-            description = ' and '.join(description[:-2].rsplit(', ', 1))
-
-            artists = list(map(lambda x: requests.get_request(
-                url=f'https://api.spotify.com/v1/search?q={x}&type=artist&limit=1', headers=self.__headers).json()['artists']['items'][0]['id'], artists_info))
-            url += f'&seed_artists={",".join(artists)}'
-
-            if len(artists_info) == 1:
-                description = description.replace('artists', 'artist')
-
-        if genres_info:
-            types.append('genres')
-            url += f'&seed_genres={",".join(genres_info)}'
-
-            if artists_info and not tracks_info:
-                description += ', and the genres '
-                final_sep = ''
-            elif not artists_info and tracks_info:
-                description += 'the genres '
-                final_sep = ', and the tracks '
-            elif not (artists_info or tracks_info):
-                description += 'the genres '
-                final_sep = ''
-            else:  # both artists and tracks exist
-                description += ', the genres '
-                final_sep = ', and the tracks '
-
-            for genre in genres_info:
-                description += f'{genre}, '
-
-            description = f"{' and '.join(description[:-2].rsplit(', ', 1)) if len(genres_info) > 1 else description[:-2]}{final_sep}"
-
-            if len(genres_info) == 1:
-                description = description.replace('genres', 'genre')
-
-        if tracks_info:
-            types.append('tracks')
-            if artists_info and not genres_info:
-                description += ', and the tracks '
-            elif not artists_info and not genres_info:
-                description += 'the tracks '
-
-            if isinstance(tracks_info, dict):
-                for song, artist in tracks_info.items():
-                    description += f'{song} by {artist}, '
-
-                tracks = [requests.get_request(url=f'https://api.spotify.com/v1/search?q={song} {artist}&type=track&limit=1', headers=self.__headers).json()[
-                    'tracks']['items'][0]['id'] for song, artist in tracks_info.items()]
-
-            elif isinstance(tracks_info[0], tuple) or isinstance(tracks_info[0], list):
-                for song, artist in tracks_info:
-                    description += f'{song} by {artist}, '
-                tracks = [requests.get_request(url=f'https://api.spotify.com/v1/search?q={song} {artist}&type=track&limit=1', headers=self.__headers).json()[
-                    'tracks']['items'][0]['id'] for song, artist in tracks_info]
-
-            elif isinstance(tracks_info[0], str):
-                for song in tracks_info:
-                    description += f'{song}, '
-                tracks = [requests.get_request(url=f'https://api.spotify.com/v1/search?q={song}&type=track&limit=1', headers=self.__headers).json()[
-                    'tracks']['items'][0]['id'] for song in tracks_info]
-
-            else:
-                raise ValueError(
-                    'The argument tracks_info must be an instance of one of the following 4 types: list[str], list[tuple[str]], list[list[str]], dict[str, str]')
-
-            description = ' and '.join(
-                description[:-2].rsplit(', ', 1)) if len(artists_info) > 1 else description[:-2]
+        for _ in range(2):
+            try:
 
-            url += f'&seed_tracks={",".join(tracks)}'
+                if artists_info:
+                    types.append('artists')
+                    description += 'the artists '
+                    for artist in artists_info:
+                        description += f'{artist}, '
+
+                    description = ' and '.join(description[:-2].rsplit(', ', 1))
+
+                    artists = list(map(lambda x: requests.get_request(
+                        url=f'https://api.spotify.com/v1/search?q={x}&type=artist&limit=1', headers=self.__headers).json()['artists']['items'][0]['id'], artists_info))
+                    url += f'&seed_artists={",".join(artists)}'
+
+                    if len(artists_info) == 1:
+                        description = description.replace('artists', 'artist')
+
+                if genres_info:
+                    types.append('genres')
+                    url += f'&seed_genres={",".join(genres_info)}'
+
+                    if artists_info and not tracks_info:
+                        description += ', and the genres '
+                        final_sep = ''
+                    elif not artists_info and tracks_info:
+                        description += 'the genres '
+                        final_sep = ', and the tracks '
+                    elif not (artists_info or tracks_info):
+                        description += 'the genres '
+                        final_sep = ''
+                    else:  # both artists and tracks exist
+                        description += ', the genres '
+                        final_sep = ', and the tracks '
+
+                    for genre in genres_info:
+                        description += f'{genre}, '
+
+                    description = f"{' and '.join(description[:-2].rsplit(', ', 1)) if len(genres_info) > 1 else description[:-2]}{final_sep}"
+
+                    if len(genres_info) == 1:
+                        description = description.replace('genres', 'genre')
+
+                if tracks_info:
+                    types.append('tracks')
+                    if artists_info and not genres_info:
+                        description += ', and the tracks '
+                    elif not artists_info and not genres_info:
+                        description += 'the tracks '
+
+                    if isinstance(tracks_info, dict):
+                        for song, artist in tracks_info.items():
+                            description += f'{song} by {artist}, '
+
+                        tracks = [requests.get_request(url=f'https://api.spotify.com/v1/search?q={song} {artist}&type=track&limit=1', headers=self.__headers).json()[
+                            'tracks']['items'][0]['id'] for song, artist in tracks_info.items()]
+
+                    elif isinstance(tracks_info[0], tuple) or isinstance(tracks_info[0], list):
+                        for song, artist in tracks_info:
+                            description += f'{song} by {artist}, '
+                        tracks = [requests.get_request(url=f'https://api.spotify.com/v1/search?q={song} {artist}&type=track&limit=1', headers=self.__headers).json()[
+                            'tracks']['items'][0]['id'] for song, artist in tracks_info]
+
+                    elif isinstance(tracks_info[0], str):
+                        for song in tracks_info:
+                            description += f'{song}, '
+                        tracks = [requests.get_request(url=f'https://api.spotify.com/v1/search?q={song}&type=track&limit=1', headers=self.__headers).json()[
+                            'tracks']['items'][0]['id'] for song in tracks_info]
+
+                    else:
+                        raise ValueError(
+                            'The argument tracks_info must be an instance of one of the following 4 types: list[str], list[tuple[str]], list[list[str]], dict[str, str]')
+
+                    description = ' and '.join(
+                        description[:-2].rsplit(', ', 1)) if len(artists_info) > 1 else description[:-2]
+
+                    url += f'&seed_tracks={",".join(tracks)}'
+
+                    if len(tracks_info) == 1:
+                        description = description.replace('tracks', 'track')
+
+                if use_main_playlist_audio_features:
+
+                    audio_statistics = self.audio_features_statistics()
+
+                    min_tempo = audio_statistics['min_tempo'] * 0.8
+                    max_tempo = audio_statistics['max_tempo'] * 1.2
+                    target_tempo = audio_statistics['mean_tempo']
+                    min_energy = audio_statistics['min_energy'] * 0.8
+                    max_energy = audio_statistics['max_energy'] * 1.2
+                    target_energy = audio_statistics['mean_energy']
+                    min_valence = audio_statistics['min_valence'] * 0.8
+                    max_valence = audio_statistics['max_valence'] * 1.2
+                    target_valence = audio_statistics['mean_valence']
+                    min_danceability = audio_statistics['min_danceability'] * 0.8
+                    max_danceability = audio_statistics['max_danceability'] * 1.2
+                    target_danceability = audio_statistics['mean_danceability']
+                    min_instrumentalness = audio_statistics['min_instrumentalness'] * 0.8
+                    max_instrumentalness = audio_statistics['max_instrumentalness'] * 1.2
+                    target_instrumentalness = audio_statistics['mean_instrumentalness']
+
+                    url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
+
+                recommendations = requests.get_request(
+                    url=url, headers=self.__headers).json()
+
+                songs = []
+
+                for song in recommendations["tracks"]:
+                    (id, name, popularity, artist), song_genres = util.song_data(
+                        song=song, added_at=False), self.__get_song_genres(song)
+                    song['id'] = id
+                    danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
+                        song=song, headers=self.__headers)
+                    songs.append({
+                        "id": id,
+                        "name": name,
+                        "artists": artist,
+                        "popularity": popularity,
+                        "genres": song_genres,
+                        "danceability": danceability,
+                        "energy": energy,
+                        "instrumentalness": instrumentalness,
+                        "tempo": tempo,
+                        "valence": valence
+                    })
 
-            if len(tracks_info) == 1:
-                description = description.replace('tracks', 'track')
-
-        if use_main_playlist_audio_features:
-
-            audio_statistics = self.audio_features_statistics()
-
-            min_tempo = audio_statistics['min_tempo'] * 0.8
-            max_tempo = audio_statistics['max_tempo'] * 1.2
-            target_tempo = audio_statistics['mean_tempo']
-            min_energy = audio_statistics['min_energy'] * 0.8
-            max_energy = audio_statistics['max_energy'] * 1.2
-            target_energy = audio_statistics['mean_energy']
-            min_valence = audio_statistics['min_valence'] * 0.8
-            max_valence = audio_statistics['max_valence'] * 1.2
-            target_valence = audio_statistics['mean_valence']
-            min_danceability = audio_statistics['min_danceability'] * 0.8
-            max_danceability = audio_statistics['max_danceability'] * 1.2
-            target_danceability = audio_statistics['mean_danceability']
-            min_instrumentalness = audio_statistics['min_instrumentalness'] * 0.8
-            max_instrumentalness = audio_statistics['max_instrumentalness'] * 1.2
-            target_instrumentalness = audio_statistics['mean_instrumentalness']
-
-            url += f'&{min_tempo=!s}&{max_tempo=!s}&{target_tempo=!s}&{min_energy=!s}&{max_energy=!s}&{target_energy=!s}&{min_valence=!s}&{max_valence=!s}&{target_valence=!s}&{min_danceability=!s}&{max_danceability=!s}&{target_danceability=!s}&{min_instrumentalness=!s}&{max_instrumentalness=!s}&{target_instrumentalness=!s}'
-
-        recommendations = requests.get_request(
-            url=url, headers=self.__headers).json()
-
-        songs = []
-
-        for song in recommendations["tracks"]:
-            (id, name, popularity, artist), song_genres = util.song_data(
-                song=song, added_at=False), self.__get_song_genres(song)
-            song['id'] = id
-            danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
-                song=song, headers=self.__headers)
-            songs.append({
-                "id": id,
-                "name": name,
-                "artists": artist,
-                "popularity": popularity,
-                "genres": song_genres,
-                "danceability": danceability,
-                "energy": energy,
-                "instrumentalness": instrumentalness,
-                "tempo": tempo,
-                "valence": valence
-            })
+                recommendations_playlist = pd.DataFrame(data=songs)
 
-        recommendations_playlist = pd.DataFrame(data=songs)
+                if build_playlist:
+                    ids = recommendations_playlist['id'].tolist()
+                    types = ' and '.join(', '.join(types).rsplit(
+                        ', ', 1)) if len(types) > 1 else types[0]
+                    self.__general_recommendation_description = description
+                    self.__general_recommendation_description_types = types
+
+                    self.__write_playlist(
+                        K=K,
+                        type='general-recommendation',
+                        additional_info=ids
+                    )
+            except AccessTokenExpiredError as e:
+                print('Error due to the access token expiration')
+                auth_token = auth.refresh_token()
 
-        if build_playlist:
-            ids = recommendations_playlist['id'].tolist()
-            types = ' and '.join(', '.join(types).rsplit(
-                ', ', 1)) if len(types) > 1 else types[0]
-            self.__general_recommendation_description = description
-            self.__general_recommendation_description_types = types
+                self.__auth_token = auth_token
 
-            self.__write_playlist(
-                K=K,
-                type='general-recommendation',
-                additional_info=ids
-            )
+                self.__headers['Authorization'] = f'Bearer {auth_token}'
+            else:
+                break
 
         return recommendations_playlist
 
 
 def start_api(user_id, *, playlist_url=None, playlist_id=None):
     """Function that prepares for and initializes the API
 
@@ -1854,15 +1926,12 @@
         raise ValueError(
             'It is necessary to specify a playlist either with playlist id or playlist url')
     if not playlist_id:
         playlist_id = False
     else:
         playlist_url = False
 
-    get_auth()
-    auth_token = input('Paste here the auth token: ')
-    while not auth_token:
-        auth_token = input('Enter a valid auth token: ')
+    print('Retrieving Authentication token')
 
-    auth_token = f'Bearer {auth_token}'
+    auth_token = f'Bearer {auth.get_auth()}'
 
     return SpotifyAPI(auth_token=auth_token, playlist_id=playlist_id, user_id=user_id, playlist_url=playlist_url)
```

## spotify_recommender_api/request_handler.py

```diff
@@ -1,11 +1,11 @@
 import json
 import time
 from requests import get, post, delete, put
-from spotify_recommender_api.error import HTTPRequestError, TooManyRequestsError
+from spotify_recommender_api.error import HTTPRequestError, TooManyRequestsError, AccessTokenExpiredError
 
 
 def exponential_backoff(func, retries: int = 5, *args, **kwargs):
     """Exponential backoff strategy (https://en.wikipedia.org/wiki/Exponential_backoff)
     in order to retry certain function after exponetially increasing delay, to overcome "429: Too Many Requests" error
 
     Args:
@@ -30,14 +30,18 @@
                 if response.status_code != 204 and 'error' in response.json():
                     raise HTTPRequestError(func_name=func.__name__, err_code=f"{response.json()['error']['status']}: {response.json()['error']['message']}", message=None, *args, **kwargs)
             return response
         except Exception as e:
             if any(errorCode in f'{e}' for errorCode in ['404', '50']):
                 continue
 
+            if '401' in f'{e}':
+                print('Access Token Expired')
+                raise AccessTokenExpiredError(func_name=func.__name__, err_code=f"{response.json()['error']['status']}: {response.json()['error']['message']}", message=None, *args, **kwargs) from e
+
             if '429' not in f'{e}':
                 raise HTTPRequestError(func_name=func.__name__, err_code=f"{response.json()['error']['status']}: {response.json()['error']['message']}", message=None, *args, **kwargs) from e
 
             if x == 0:
                 print('\nExponential backoff triggered: ')
 
             x += 1
@@ -73,14 +77,42 @@
         retries (int, optional): Number of retries. Defaults to 10.
 
     Returns:
         dict: Request response
     """
     return exponential_backoff(func=post, url=url, headers=headers, data=json.dumps(data), retries=retries)
 
+def post_request_dict(url: str, headers: dict = None, data: dict = None, retries: int = 10) -> dict:
+    """POST request with integrated exponential backoff retry strategy
+
+    Args:
+        url (str): Request URL
+        headers (dict, optional): Request headers. Defaults to None.
+        data (dict, optional): Request body. Defaults to None.
+        retries (int, optional): Number of retries. Defaults to 10.
+
+    Returns:
+        dict: Request response
+    """
+    return exponential_backoff(func=post, url=url, headers=headers, data=data, retries=retries)
+
+def post_request_with_auth(url: str, headers: dict = None, data: dict = None, auth: 'tuple[str]' = None, retries: int = 10) -> dict:
+    """POST request with integrated exponential backoff retry strategy
+
+    Args:
+        url (str): Request URL
+        headers (dict, optional): Request headers. Defaults to None.
+        data (dict, optional): Request body. Defaults to None.
+        retries (int, optional): Number of retries. Defaults to 10.
+
+    Returns:
+        dict: Request response
+    """
+    return exponential_backoff(func=post, url=url, headers=headers, data=data, auth=auth, retries=retries)
+
 def put_request(url: str, headers: dict = None, data: dict = None, retries: int = 10) -> dict:
     """PUT request with integrated exponential backoff retry strategy
 
     Args:
         url (str): Request URL
         headers (dict, optional): Request headers. Defaults to None.
         data (dict, optional): Request body. Defaults to None.
```

## spotify_recommender_api/util.py

```diff
@@ -245,12 +245,11 @@
     """This is a decorator which can be used to mark functions
     as deprecated. It will result in a warning being emitted
     when the function is used."""
 
     @functools.wraps(func)
     def new_func(*args, **kwargs):
         warnings.simplefilter('always', DeprecationWarning)  # turn off filter
-        warnings.warn(
-            f"Call to deprecated function {func.__name__}.", category=DeprecationWarning, stacklevel=2)
+        warnings.warn(f"Call to deprecated function {func.__name__}.", category=DeprecationWarning, stacklevel=2)
         warnings.simplefilter('default', DeprecationWarning)  # reset filter
         return func(*args, **kwargs)
     return new_func
```

## Comparing `spotify_recommender_api-3.9.5.dist-info/METADATA` & `spotify_recommender_api-4.0.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: spotify-recommender-api
-Version: 3.9.5
+Version: 4.0.0
 Summary: Python package which takes the songs of a greater playlist as starting point to make recommendations of groups of songs that might bond well within that same playlist, using K-Nearest-Neighbors Technique
 Home-page: https://github.com/nikolas-virionis/spotify-api
 Author: Nikolas B Virionis
 Author-email: nikolas.virionis@bandtec.com.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+Requires-Dist: fastapi
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: seaborn
+Requires-Dist: uvicorn
 
 
 # spotify-recommender
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spotify-recommender-api?style=plastic)
 ![PyPI](https://img.shields.io/pypi/v/spotify-recommender-api?style=plastic)
 ![GitHub repo size](https://img.shields.io/github/repo-size/nikolas-virionis/spotify-api)
 ![GitHub last commit](https://img.shields.io/github/last-commit/nikolas-virionis/spotify-api?style=plastic)
```

## Comparing `spotify_recommender_api-3.9.5.dist-info/RECORD` & `spotify_recommender_api-4.0.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-spotify_recommender_api/__init__.py,sha256=U1-uNHEYMelaKSlNJc-B0UAazVXk5IOEQHaAY6T59aI,21
-spotify_recommender_api/authentication.py,sha256=CsBSlV-0ArGxxcVilKZn875GkD7HoHQ6jJhCZHYrpss,927
+spotify_recommender_api/__init__.py,sha256=6C4WlnzpBkuaIQfXufNhBcHodFiDNdiuXZ7W2zngE6U,21
+spotify_recommender_api/authentication.py,sha256=SRLj_deiGKs-elwzarGPSK9hnfzfveStBFZPk8HktKY,1303
 spotify_recommender_api/core.py,sha256=LXwBE6Z9npgglH2Jt9e6HQthe2g3XbJcJpDVTh-Jf24,14242
-spotify_recommender_api/error.py,sha256=Axvd59i8GE9N-5Pcs_EUGHh5LVAvAPkRkU4YKgqqglk,1320
-spotify_recommender_api/recommender.py,sha256=G_A7TFXzpP0AYsXb7AjbPOV8-qQVat2HOpJ7cyDRTz4,87641
-spotify_recommender_api/request_handler.py,sha256=FqWl1TKjT-WMkI_GLGORYeYuD29NCx5N8N3Kq-xRTTM,4393
+spotify_recommender_api/error.py,sha256=KSVWVMZxXshQlHHzrDkSilDOfavtSIY_ZiyQ4opFai4,1966
+spotify_recommender_api/recommender.py,sha256=F1ViSjvyV_KPHcULsOU98uAFf_eeVDjb_CVyJ1XcK0s,91849
+spotify_recommender_api/request_handler.py,sha256=NQa5jdpw6tD_PS1Bx_aTNtV_X-pZj0hSB9GAkOKW0A0,5866
 spotify_recommender_api/sensitive.py,sha256=Xn2FFn4uUk94Ei_It1U2iT5ZZEafHBt9q--lSPwlaoI,99
-spotify_recommender_api/util.py,sha256=xa1SDP1KWWGH604sV3NA12LE1LdxzywakX33Vx94uoI,9124
-spotify_recommender_api-3.9.5.dist-info/METADATA,sha256=MgQ7VtGiYOme3ruYHeiNgy0KI3KbqZh9fHMSnzEUY74,20775
-spotify_recommender_api-3.9.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-spotify_recommender_api-3.9.5.dist-info/top_level.txt,sha256=X65Ob3YNye88oWqQCXBvKpEUdmLQvio-wg4Ra2Gsh-c,24
-spotify_recommender_api-3.9.5.dist-info/RECORD,,
+spotify_recommender_api/server.py,sha256=4qKBIw6iZymSjOy4L_oEnLC3AdLaJZKzG6VkafAnzmU,6637
+spotify_recommender_api/util.py,sha256=GMof5qAKZu3F0R1ze-R0j0tsK7cQhKvKiDCbziwSkio,9111
+spotify_recommender_api-4.0.0.dist-info/METADATA,sha256=unTpFUC9oj0MLPG4d42qbZZf-IByI75_-rd-hLMz2UA,20821
+spotify_recommender_api-4.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+spotify_recommender_api-4.0.0.dist-info/top_level.txt,sha256=X65Ob3YNye88oWqQCXBvKpEUdmLQvio-wg4Ra2Gsh-c,24
+spotify_recommender_api-4.0.0.dist-info/RECORD,,
```

