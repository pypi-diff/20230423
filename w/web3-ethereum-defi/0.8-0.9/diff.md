# Comparing `tmp/web3-ethereum-defi-0.8.tar.gz` & `tmp/web3-ethereum-defi-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3-ethereum-defi-0.8.tar", max compression
+gzip compressed data, was "web3-ethereum-defi-0.9.tar", max compression
```

## Comparing `web3-ethereum-defi-0.8.tar` & `web3-ethereum-defi-0.9.tar`

### file list

```diff
@@ -1,242 +1,250 @@
--rw-r--r--   0        0        0     1059 2022-04-04 18:53:58.088251 web3-ethereum-defi-0.8/LICENSE.txt
--rw-r--r--   0        0        0    10199 2022-04-07 10:40:21.178665 web3-ethereum-defi-0.8/README.md
--rw-r--r--   0        0        0     6145 2022-04-04 19:20:04.934944 web3-ethereum-defi-0.8/eth_defi/abi/BaseBoringBatchable.json
--rw-r--r--   0        0        0    97771 2022-04-04 19:20:04.964160 web3-ethereum-defi-0.8/eth_defi/abi/BentoBoxV1.json
--rw-r--r--   0        0        0     8730 2022-04-04 19:20:04.943822 web3-ethereum-defi-0.8/eth_defi/abi/BoringBatchable.json
--rw-r--r--   0        0        0      665 2022-04-04 19:20:04.996210 web3-ethereum-defi-0.8/eth_defi/abi/BoringERC20.json
--rw-r--r--   0        0        0     5849 2022-04-04 19:20:04.957751 web3-ethereum-defi-0.8/eth_defi/abi/BoringFactory.json
--rw-r--r--   0        0        0      664 2022-04-04 19:20:04.998247 web3-ethereum-defi-0.8/eth_defi/abi/BoringMath.json
--rw-r--r--   0        0        0      667 2022-04-04 19:20:04.989692 web3-ethereum-defi-0.8/eth_defi/abi/BoringMath128.json
--rw-r--r--   0        0        0      655 2022-04-04 19:20:04.969959 web3-ethereum-defi-0.8/eth_defi/abi/BoringMath32.json
--rw-r--r--   0        0        0      655 2022-04-04 19:20:04.967997 web3-ethereum-defi-0.8/eth_defi/abi/BoringMath64.json
--rw-r--r--   0        0        0     5657 2022-04-04 19:20:05.008085 web3-ethereum-defi-0.8/eth_defi/abi/BoringOwnable.json
--rw-r--r--   0        0        0     1590 2022-04-04 19:20:05.009994 web3-ethereum-defi-0.8/eth_defi/abi/BoringOwnableData.json
--rw-r--r--   0        0        0    37476 2022-04-04 19:20:04.864152 web3-ethereum-defi-0.8/eth_defi/abi/CloneRewarderTime.json
--rw-r--r--   0        0        0    45593 2022-04-04 19:20:04.879841 web3-ethereum-defi-0.8/eth_defi/abi/CloneRewarderTimeDual.json
--rw-r--r--   0        0        0    38288 2022-04-04 19:20:04.872905 web3-ethereum-defi-0.8/eth_defi/abi/ComplexRewarder.json
--rw-r--r--   0        0        0    39055 2022-04-04 19:20:04.870674 web3-ethereum-defi-0.8/eth_defi/abi/ComplexRewarderTime.json
--rw-r--r--   0        0        0     2394 2022-04-04 19:20:04.979904 web3-ethereum-defi-0.8/eth_defi/abi/Domain.json
--rw-r--r--   0        0        0    16310 2022-04-04 19:20:05.012113 web3-ethereum-defi-0.8/eth_defi/abi/ERC20.json
--rw-r--r--   0        0        0     3089 2022-04-04 19:20:05.006055 web3-ethereum-defi-0.8/eth_defi/abi/ERC20Data.json
--rw-r--r--   0        0        0    18473 2022-04-04 19:20:04.868423 web3-ethereum-defi-0.8/eth_defi/abi/ERC20Mock.json
--rw-r--r--   0        0        0    18679 2022-04-04 19:20:05.025670 web3-ethereum-defi-0.8/eth_defi/abi/ERC20MockDecimals.json
--rw-r--r--   0        0        0     1002 2022-04-04 19:20:05.000005 web3-ethereum-defi-0.8/eth_defi/abi/IBatchFlashBorrower.json
--rw-r--r--   0        0        0    24473 2022-04-04 19:20:05.001965 web3-ethereum-defi-0.8/eth_defi/abi/IBentoBoxV1.json
--rw-r--r--   0        0        0     1204 2022-04-04 19:20:05.019713 web3-ethereum-defi-0.8/eth_defi/abi/IBentoBoxWithdraw.json
--rw-r--r--   0        0        0     3831 2022-04-04 19:20:05.055716 web3-ethereum-defi-0.8/eth_defi/abi/IERC20.json
--rw-r--r--   0        0        0     4737 2022-04-04 19:20:04.914932 web3-ethereum-defi-0.8/eth_defi/abi/IERC20Uniswap.json
--rw-r--r--   0        0        0      977 2022-04-04 19:20:04.985658 web3-ethereum-defi-0.8/eth_defi/abi/IFlashBorrower.json
--rw-r--r--   0        0        0     1513 2022-04-04 19:20:05.017899 web3-ethereum-defi-0.8/eth_defi/abi/IKashiWithdrawFee.json
--rw-r--r--   0        0        0     1873 2022-04-04 19:20:05.060868 web3-ethereum-defi-0.8/eth_defi/abi/IMasterChef.json
--rw-r--r--   0        0        0      636 2022-04-04 19:20:04.877101 web3-ethereum-defi-0.8/eth_defi/abi/IMasterChefV2.json
--rw-r--r--   0        0        0      508 2022-04-04 19:20:04.983719 web3-ethereum-defi-0.8/eth_defi/abi/IMasterContract.json
--rw-r--r--   0        0        0      504 2022-04-04 19:20:04.912914 web3-ethereum-defi-0.8/eth_defi/abi/IMigrator.json
--rw-r--r--   0        0        0      627 2022-04-04 19:20:05.045376 web3-ethereum-defi-0.8/eth_defi/abi/IMigratorChef.json
--rw-r--r--   0        0        0     4157 2022-04-04 19:20:05.062888 web3-ethereum-defi-0.8/eth_defi/abi/IMiniChefV2.json
--rw-r--r--   0        0        0     2296 2022-04-04 19:20:04.987743 web3-ethereum-defi-0.8/eth_defi/abi/IOracle.json
--rw-r--r--   0        0        0     1703 2022-04-04 19:20:05.057630 web3-ethereum-defi-0.8/eth_defi/abi/IRewarder.json
--rw-r--r--   0        0        0     1786 2022-04-04 19:20:05.003955 web3-ethereum-defi-0.8/eth_defi/abi/IStrategy.json
--rw-r--r--   0        0        0     2362 2022-04-04 19:20:04.991734 web3-ethereum-defi-0.8/eth_defi/abi/ISwapper.json
--rw-r--r--   0        0        0      872 2022-04-04 19:20:04.931362 web3-ethereum-defi-0.8/eth_defi/abi/IUniswapV2Callee.json
--rw-r--r--   0        0        0     6564 2022-04-04 19:20:04.918845 web3-ethereum-defi-0.8/eth_defi/abi/IUniswapV2ERC20.json
--rw-r--r--   0        0        0     4095 2022-04-04 19:20:04.926404 web3-ethereum-defi-0.8/eth_defi/abi/IUniswapV2Factory.json
--rw-r--r--   0        0        0    13664 2022-04-04 19:20:04.929326 web3-ethereum-defi-0.8/eth_defi/abi/IUniswapV2Pair.json
--rw-r--r--   0        0        0    16744 2022-04-04 19:20:04.916872 web3-ethereum-defi-0.8/eth_defi/abi/IUniswapV2Router01.json
--rw-r--r--   0        0        0    21403 2022-04-04 19:20:04.920998 web3-ethereum-defi-0.8/eth_defi/abi/IUniswapV2Router02.json
--rw-r--r--   0        0        0      634 2022-04-04 19:20:04.966013 web3-ethereum-defi-0.8/eth_defi/abi/IWETH.json
--rw-r--r--   0        0        0   122472 2022-04-04 19:20:04.981862 web3-ethereum-defi-0.8/eth_defi/abi/KashiPairMediumRiskV1.json
--rw-r--r--   0        0        0     3162 2022-04-04 19:20:05.052003 web3-ethereum-defi-0.8/eth_defi/abi/MalformedERC20.json
--rw-r--r--   0        0        0    41078 2022-04-04 19:20:05.043690 web3-ethereum-defi-0.8/eth_defi/abi/MasterChef.json
--rw-r--r--   0        0        0    68638 2022-04-04 19:20:05.037805 web3-ethereum-defi-0.8/eth_defi/abi/MasterChefV2.json
--rw-r--r--   0        0        0    25138 2022-04-04 19:20:04.955814 web3-ethereum-defi-0.8/eth_defi/abi/MasterContractManager.json
--rw-r--r--   0        0        0      652 2022-04-04 19:20:04.904354 web3-ethereum-defi-0.8/eth_defi/abi/Math.json
--rw-r--r--   0        0        0     9753 2022-04-04 19:20:04.886002 web3-ethereum-defi-0.8/eth_defi/abi/Migrator.json
--rw-r--r--   0        0        0    64126 2022-04-04 19:20:04.888196 web3-ethereum-defi-0.8/eth_defi/abi/MiniChefV2.json
--rw-r--r--   0        0        0    16797 2022-04-04 19:20:05.053888 web3-ethereum-defi-0.8/eth_defi/abi/Multicall2.json
--rw-r--r--   0        0        0     1790 2022-04-04 19:20:05.023680 web3-ethereum-defi-0.8/eth_defi/abi/Ownable.json
--rw-r--r--   0        0        0     1511 2022-04-04 19:20:05.021830 web3-ethereum-defi-0.8/eth_defi/abi/OwnableData.json
--rw-r--r--   0        0        0     6464 2022-04-04 19:20:04.975672 web3-ethereum-defi-0.8/eth_defi/abi/PeggedOracleV1.json
--rw-r--r--   0        0        0      667 2022-04-04 19:20:04.993600 web3-ethereum-defi-0.8/eth_defi/abi/RebaseLibrary.json
--rw-r--r--   0        0        0     3335 2022-04-04 19:20:04.883945 web3-ethereum-defi-0.8/eth_defi/abi/RewarderBrokenMock.json
--rw-r--r--   0        0        0     8849 2022-04-04 19:20:04.855298 web3-ethereum-defi-0.8/eth_defi/abi/RewarderMock.json
--rw-r--r--   0        0        0     2454 2022-04-04 19:20:05.027651 web3-ethereum-defi-0.8/eth_defi/abi/SafeERC20.json
--rw-r--r--   0        0        0      650 2022-04-04 19:20:05.029722 web3-ethereum-defi-0.8/eth_defi/abi/SafeMath.json
--rw-r--r--   0        0        0      653 2022-04-04 19:20:05.032685 web3-ethereum-defi-0.8/eth_defi/abi/SafeMath128.json
--rw-r--r--   0        0        0      667 2022-04-04 19:20:04.900089 web3-ethereum-defi-0.8/eth_defi/abi/SafeMathUniswap.json
--rw-r--r--   0        0        0      662 2022-04-04 19:20:05.034682 web3-ethereum-defi-0.8/eth_defi/abi/SignedSafeMath.json
--rw-r--r--   0        0        0    24381 2022-04-04 19:20:04.933124 web3-ethereum-defi-0.8/eth_defi/abi/SushiBar.json
--rw-r--r--   0        0        0    29251 2022-04-04 19:20:05.047088 web3-ethereum-defi-0.8/eth_defi/abi/SushiMaker.json
--rw-r--r--   0        0        0     2896 2022-04-04 19:20:04.881895 web3-ethereum-defi-0.8/eth_defi/abi/SushiMakerExploitMock.json
--rw-r--r--   0        0        0    21943 2022-04-04 19:20:05.016033 web3-ethereum-defi-0.8/eth_defi/abi/SushiMakerKashi.json
--rw-r--r--   0        0        0     2715 2022-04-04 19:20:04.875020 web3-ethereum-defi-0.8/eth_defi/abi/SushiMakerKashiExploitMock.json
--rw-r--r--   0        0        0    20673 2022-04-04 19:20:04.892126 web3-ethereum-defi-0.8/eth_defi/abi/SushiRoll.json
--rw-r--r--   0        0        0    49829 2022-04-04 19:20:04.861749 web3-ethereum-defi-0.8/eth_defi/abi/SushiSwapFactoryMock.json
--rw-r--r--   0        0        0    50610 2022-04-04 19:20:04.859593 web3-ethereum-defi-0.8/eth_defi/abi/SushiSwapPairMock.json
--rw-r--r--   0        0        0    41108 2022-04-04 19:20:05.041843 web3-ethereum-defi-0.8/eth_defi/abi/SushiToken.json
--rw-r--r--   0        0        0    34840 2022-04-04 19:20:05.050003 web3-ethereum-defi-0.8/eth_defi/abi/Timelock.json
--rw-r--r--   0        0        0      672 2022-04-04 19:20:04.906395 web3-ethereum-defi-0.8/eth_defi/abi/TransferHelper.json
--rw-r--r--   0        0        0      662 2022-04-04 19:20:04.901974 web3-ethereum-defi-0.8/eth_defi/abi/UQ112x112.json
--rw-r--r--   0        0        0    15775 2022-04-04 19:20:04.896411 web3-ethereum-defi-0.8/eth_defi/abi/UniswapV2ERC20.json
--rw-r--r--   0        0        0    49825 2022-04-04 19:20:04.894263 web3-ethereum-defi-0.8/eth_defi/abi/UniswapV2Factory.json
--rw-r--r--   0        0        0      676 2022-04-04 19:20:04.898316 web3-ethereum-defi-0.8/eth_defi/abi/UniswapV2Library.json
--rw-r--r--   0        0        0    50606 2022-04-04 19:20:04.910703 web3-ethereum-defi-0.8/eth_defi/abi/UniswapV2Pair.json
--rw-r--r--   0        0        0    93624 2022-04-04 19:20:04.908544 web3-ethereum-defi-0.8/eth_defi/abi/UniswapV2Router02.json
--rw-r--r--   0        0        0    14171 2022-04-04 19:20:04.857711 web3-ethereum-defi-0.8/eth_defi/abi/WETH9Mock.json
--rw-r--r--   0        0        0     5423 2022-04-04 18:53:58.106078 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/Base64Test.json
--rw-r--r--   0        0        0      484 2022-04-04 18:53:58.106166 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/BitMath.json
--rw-r--r--   0        0        0     3518 2022-04-04 18:53:58.106283 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/BitMathEchidnaTest.json
--rw-r--r--   0        0        0     4755 2022-04-04 18:53:58.106403 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/BitMathTest.json
--rw-r--r--   0        0        0      243 2022-04-04 18:53:58.106487 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/BlockTimestamp.json
--rw-r--r--   0        0        0      486 2022-04-04 18:53:58.106556 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/BytesLib.json
--rw-r--r--   0        0        0      506 2022-04-04 18:53:58.106636 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/CallbackValidation.json
--rw-r--r--   0        0        0      484 2022-04-04 18:53:58.106703 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/ChainId.json
--rw-r--r--   0        0        0     9758 2022-04-04 18:53:58.106823 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/ERC721Permit.json
--rw-r--r--   0        0        0      496 2022-04-04 18:53:58.106904 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/FixedPoint128.json
--rw-r--r--   0        0        0      494 2022-04-04 18:53:58.106978 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/FixedPoint96.json
--rw-r--r--   0        0        0      486 2022-04-04 18:53:58.107047 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/FullMath.json
--rw-r--r--   0        0        0     4959 2022-04-04 18:53:58.107242 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/FullMathEchidnaTest.json
--rw-r--r--   0        0        0     3245 2022-04-04 18:53:58.107347 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/FullMathTest.json
--rw-r--r--   0        0        0      490 2022-04-04 18:53:58.107419 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/HexStrings.json
--rw-r--r--   0        0        0      747 2022-04-04 18:53:58.107522 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IERC1271.json
--rw-r--r--   0        0        0     4757 2022-04-04 18:53:58.107669 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IERC20Metadata.json
--rw-r--r--   0        0        0     3758 2022-04-04 18:53:58.107762 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IERC20Minimal.json
--rw-r--r--   0        0        0     1306 2022-04-04 18:53:58.107839 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IERC20PermitAllowed.json
--rw-r--r--   0        0        0     7547 2022-04-04 18:53:58.107931 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IERC721Permit.json
--rw-r--r--   0        0        0      624 2022-04-04 18:53:58.108044 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IMulticall.json
--rw-r--r--   0        0        0    22092 2022-04-04 18:53:58.108468 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/INonfungiblePositionManager.json
--rw-r--r--   0        0        0     1228 2022-04-04 18:53:58.108658 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/INonfungibleTokenPositionDescriptor.json
--rw-r--r--   0        0        0      771 2022-04-04 18:53:58.108853 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IPeripheryImmutableState.json
--rw-r--r--   0        0        0     1289 2022-04-04 18:53:58.109283 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IPeripheryPayments.json
--rw-r--r--   0        0        0     2675 2022-04-04 18:53:58.109373 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IPeripheryPaymentsWithFee.json
--rw-r--r--   0        0        0     1003 2022-04-04 18:53:58.109474 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IPoolInitializer.json
--rw-r--r--   0        0        0     2981 2022-04-04 18:53:58.109738 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IQuoter.json
--rw-r--r--   0        0        0     5081 2022-04-04 18:53:58.109834 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IQuoterV2.json
--rw-r--r--   0        0        0     3533 2022-04-04 18:53:58.109929 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/ISelfPermit.json
--rw-r--r--   0        0        0     6136 2022-04-04 18:53:58.109996 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/ISwapRouter.json
--rw-r--r--   0        0        0     1230 2022-04-04 18:53:58.110141 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/ITickLens.json
--rw-r--r--   0        0        0     4350 2022-04-04 18:53:58.110224 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3Factory.json
--rw-r--r--   0        0        0      774 2022-04-04 18:53:58.110303 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3FlashCallback.json
--rw-r--r--   0        0        0      785 2022-04-04 18:53:58.110384 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3MintCallback.json
--rw-r--r--   0        0        0    21755 2022-04-04 18:53:58.110477 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3Pool.json
--rw-r--r--   0        0        0     5058 2022-04-04 18:53:58.110592 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolActions.json
--rw-r--r--   0        0        0      980 2022-04-04 18:53:58.110671 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolDeployer.json
--rw-r--r--   0        0        0     1592 2022-04-04 18:53:58.110746 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolDerivedState.json
--rw-r--r--   0        0        0     7617 2022-04-04 18:53:58.110832 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolEvents.json
--rw-r--r--   0        0        0     1786 2022-04-04 18:53:58.110925 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolImmutables.json
--rw-r--r--   0        0        0     1426 2022-04-04 18:53:58.110996 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolOwnerActions.json
--rw-r--r--   0        0        0     5665 2022-04-04 18:53:58.111068 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolState.json
--rw-r--r--   0        0        0      783 2022-04-04 18:53:58.111142 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3SwapCallback.json
--rw-r--r--   0        0        0     6752 2022-04-04 18:53:58.111216 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IV3Migrator.json
--rw-r--r--   0        0        0     4406 2022-04-04 18:53:58.111293 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IWETH9.json
--rw-r--r--   0        0        0      502 2022-04-04 18:53:58.111366 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/LiquidityAmounts.json
--rw-r--r--   0        0        0    20362 2022-04-04 18:53:58.111477 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/LiquidityAmountsTest.json
--rw-r--r--   0        0        0     2367 2022-04-04 18:53:58.111577 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/LiquidityManagement.json
--rw-r--r--   0        0        0      496 2022-04-04 18:53:58.111647 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/LiquidityMath.json
--rw-r--r--   0        0        0     3044 2022-04-04 18:53:58.111731 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/LiquidityMathTest.json
--rw-r--r--   0        0        0      498 2022-04-04 18:53:58.111797 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/LowGasSafeMath.json
--rw-r--r--   0        0        0     4807 2022-04-04 18:53:58.111881 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/LowGasSafeMathEchidnaTest.json
--rw-r--r--   0        0        0     6854 2022-04-04 18:53:58.111977 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/MockObservable.json
--rw-r--r--   0        0        0     7231 2022-04-04 18:53:58.112056 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/MockObservations.json
--rw-r--r--   0        0        0   126981 2022-04-04 18:53:58.112232 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/MockTimeNonfungiblePositionManager.json
--rw-r--r--   0        0        0    62557 2022-04-04 18:53:58.112357 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/MockTimeSwapRouter.json
--rw-r--r--   0        0        0   113293 2022-04-04 18:53:58.112531 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/MockTimeUniswapV3Pool.json
--rw-r--r--   0        0        0    97190 2022-04-04 18:53:58.112683 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/MockTimeUniswapV3PoolDeployer.json
--rw-r--r--   0        0        0      616 2022-04-04 18:53:58.112767 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/Multicall.json
--rw-r--r--   0        0        0   100849 2022-04-04 18:53:58.113216 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NFTDescriptor.json
--rw-r--r--   0        0        0   108664 2022-04-04 18:53:58.113767 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NFTDescriptorTest.json
--rw-r--r--   0        0        0      482 2022-04-04 18:53:58.113848 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NFTSVG.json
--rw-r--r--   0        0        0      238 2022-04-04 18:53:58.113916 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NoDelegateCall.json
--rw-r--r--   0        0        0     2906 2022-04-04 18:53:58.114033 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NoDelegateCallTest.json
--rw-r--r--   0        0        0   126423 2022-04-04 18:53:58.114324 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NonfungiblePositionManager.json
--rw-r--r--   0        0        0     2289 2022-04-04 18:53:58.114426 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NonfungiblePositionManagerPositionsGasTest.json
--rw-r--r--   0        0        0    22530 2022-04-04 18:53:58.114523 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NonfungibleTokenPositionDescriptor.json
--rw-r--r--   0        0        0      482 2022-04-04 18:53:58.114598 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/Oracle.json
--rw-r--r--   0        0        0    32780 2022-04-04 18:53:58.114753 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/OracleEchidnaTest.json
--rw-r--r--   0        0        0      496 2022-04-04 18:53:58.114822 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/OracleLibrary.json
--rw-r--r--   0        0        0    28516 2022-04-04 18:53:58.114959 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/OracleTest.json
--rw-r--r--   0        0        0    30909 2022-04-04 18:53:58.115103 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PairFlash.json
--rw-r--r--   0        0        0      478 2022-04-04 18:53:58.115179 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/Path.json
--rw-r--r--   0        0        0    11849 2022-04-04 18:53:58.115256 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PathTest.json
--rw-r--r--   0        0        0      763 2022-04-04 18:53:58.115322 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PeripheryImmutableState.json
--rw-r--r--   0        0        0     2123 2022-04-04 18:53:58.115415 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PeripheryImmutableStateTest.json
--rw-r--r--   0        0        0     1854 2022-04-04 18:53:58.115472 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PeripheryPayments.json
--rw-r--r--   0        0        0     3240 2022-04-04 18:53:58.115528 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PeripheryPaymentsWithFee.json
--rw-r--r--   0        0        0      253 2022-04-04 18:53:58.115589 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PeripheryValidation.json
--rw-r--r--   0        0        0      492 2022-04-04 18:53:58.115650 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PoolAddress.json
--rw-r--r--   0        0        0     5434 2022-04-04 18:53:58.115752 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PoolAddressTest.json
--rw-r--r--   0        0        0     1495 2022-04-04 18:53:58.115826 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PoolInitializer.json
--rw-r--r--   0        0        0      502 2022-04-04 18:53:58.115880 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PoolTicksCounter.json
--rw-r--r--   0        0        0     8519 2022-04-04 18:53:58.115965 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PoolTicksCounterTest.json
--rw-r--r--   0        0        0      486 2022-04-04 18:53:58.116022 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/Position.json
--rw-r--r--   0        0        0      492 2022-04-04 18:53:58.116087 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PositionKey.json
--rw-r--r--   0        0        0      496 2022-04-04 18:53:58.116143 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PositionValue.json
--rw-r--r--   0        0        0    22712 2022-04-04 18:53:58.116248 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PositionValueTest.json
--rw-r--r--   0        0        0    23246 2022-04-04 18:53:58.116371 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/Quoter.json
--rw-r--r--   0        0        0    39940 2022-04-04 18:53:58.116528 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/QuoterV2.json
--rw-r--r--   0        0        0      486 2022-04-04 18:53:58.116600 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SafeCast.json
--rw-r--r--   0        0        0     3525 2022-04-04 18:53:58.116668 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SelfPermit.json
--rw-r--r--   0        0        0     8241 2022-04-04 18:53:58.116748 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SelfPermitTest.json
--rw-r--r--   0        0        0      496 2022-04-04 18:53:58.116808 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SqrtPriceMath.json
--rw-r--r--   0        0        0    23360 2022-04-04 18:53:58.116883 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SqrtPriceMathEchidnaTest.json
--rw-r--r--   0        0        0      510 2022-04-04 18:53:58.116951 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SqrtPriceMathPartial.json
--rw-r--r--   0        0        0    14691 2022-04-04 18:53:58.117012 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SqrtPriceMathTest.json
--rw-r--r--   0        0        0      486 2022-04-04 18:53:58.117067 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SwapMath.json
--rw-r--r--   0        0        0    10378 2022-04-04 18:53:58.117150 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SwapMathEchidnaTest.json
--rw-r--r--   0        0        0    10768 2022-04-04 18:53:58.117212 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SwapMathTest.json
--rw-r--r--   0        0        0    61914 2022-04-04 18:53:58.117312 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SwapRouter.json
--rw-r--r--   0        0        0     4049 2022-04-04 18:53:58.117402 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestCallbackValidation.json
--rw-r--r--   0        0        0    29157 2022-04-04 18:53:58.117514 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestERC20.json
--rw-r--r--   0        0        0    29989 2022-04-04 18:53:58.117628 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestERC20Metadata.json
--rw-r--r--   0        0        0    32063 2022-04-04 18:53:58.117708 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestERC20PermitAllowed.json
--rw-r--r--   0        0        0     9382 2022-04-04 18:53:58.117779 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestMulticall.json
--rw-r--r--   0        0        0     4429 2022-04-04 18:53:58.117846 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestPositionNFTOwner.json
--rw-r--r--   0        0        0    11052 2022-04-04 18:53:58.117923 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestUniswapV3Callee.json
--rw-r--r--   0        0        0    16971 2022-04-04 18:53:58.117995 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestUniswapV3ReentrantCallee.json
--rw-r--r--   0        0        0    12791 2022-04-04 18:53:58.118090 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestUniswapV3Router.json
--rw-r--r--   0        0        0     6352 2022-04-04 18:53:58.118148 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestUniswapV3SwapPay.json
--rw-r--r--   0        0        0      478 2022-04-04 18:53:58.118203 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/Tick.json
--rw-r--r--   0        0        0      490 2022-04-04 18:53:58.118259 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickBitmap.json
--rw-r--r--   0        0        0     6473 2022-04-04 18:53:58.118317 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickBitmapEchidnaTest.json
--rw-r--r--   0        0        0     8559 2022-04-04 18:53:58.118370 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickBitmapTest.json
--rw-r--r--   0        0        0     2392 2022-04-04 18:53:58.118435 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickEchidnaTest.json
--rw-r--r--   0        0        0     6826 2022-04-04 18:53:58.118509 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickLens.json
--rw-r--r--   0        0        0     7666 2022-04-04 18:53:58.118570 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickLensTest.json
--rw-r--r--   0        0        0      486 2022-04-04 18:53:58.118627 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickMath.json
--rw-r--r--   0        0        0     9186 2022-04-04 18:53:58.118711 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickMathEchidnaTest.json
--rw-r--r--   0        0        0    10809 2022-04-04 18:53:58.118791 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickMathTest.json
--rw-r--r--   0        0        0    10086 2022-04-04 18:53:58.118871 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickOverflowSafetyEchidnaTest.json
--rw-r--r--   0        0        0    19533 2022-04-04 18:53:58.118977 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickTest.json
--rw-r--r--   0        0        0      508 2022-04-04 18:53:58.119045 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TokenRatioSortOrder.json
--rw-r--r--   0        0        0      498 2022-04-04 18:53:58.119099 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TransferHelper.json
--rw-r--r--   0        0        0     7971 2022-04-04 18:53:58.119183 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/UniswapInterfaceMulticall.json
--rw-r--r--   0        0        0   104076 2022-04-04 18:53:58.119298 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/UniswapV3Factory.json
--rw-r--r--   0        0        0   111557 2022-04-04 18:53:58.119546 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/UniswapV3Pool.json
--rw-r--r--   0        0        0     2017 2022-04-04 18:53:58.119638 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/UniswapV3PoolDeployer.json
--rw-r--r--   0        0        0     6910 2022-04-04 18:53:58.119736 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/UniswapV3PoolSwapTest.json
--rw-r--r--   0        0        0      490 2022-04-04 18:53:58.119805 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/UnsafeMath.json
--rw-r--r--   0        0        0     1413 2022-04-04 18:53:58.119918 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/UnsafeMathEchidnaTest.json
--rw-r--r--   0        0        0    39457 2022-04-04 18:53:58.120015 web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/V3Migrator.json
--rw-r--r--   0        0        0     3383 2022-04-29 10:33:41.586567 web3-ethereum-defi-0.8/eth_defi/abi.py
--rw-r--r--   0        0        0     6518 2022-04-18 09:50:04.109147 web3-ethereum-defi-0.8/eth_defi/balances.py
--rw-r--r--   0        0        0     1319 2022-04-18 08:58:35.682471 web3-ethereum-defi-0.8/eth_defi/deploy.py
--rw-r--r--   0        0        0     3470 2022-04-18 09:46:34.237486 web3-ethereum-defi-0.8/eth_defi/event.py
--rw-r--r--   0        0        0    15631 2022-05-06 09:44:22.522247 web3-ethereum-defi-0.8/eth_defi/ganache.py
--rw-r--r--   0        0        0     3961 2022-04-04 18:53:58.120524 web3-ethereum-defi-0.8/eth_defi/gas.py
--rw-r--r--   0        0        0     3581 2022-05-12 13:55:30.941002 web3-ethereum-defi-0.8/eth_defi/hotwallet.py
--rw-r--r--   0        0        0     5190 2022-04-18 09:52:35.270786 web3-ethereum-defi-0.8/eth_defi/revert_reason.py
--rw-r--r--   0        0        0     6544 2022-04-30 09:18:44.826293 web3-ethereum-defi-0.8/eth_defi/token.py
--rw-r--r--   0        0        0     8574 2022-05-12 13:55:30.941518 web3-ethereum-defi-0.8/eth_defi/txmonitor.py
--rw-r--r--   0        0        0     6258 2022-04-18 09:52:05.769673 web3-ethereum-defi-0.8/eth_defi/uniswap_v2/analysis.py
--rw-r--r--   0        0        0    56174 2022-04-18 08:58:35.684049 web3-ethereum-defi-0.8/eth_defi/uniswap_v2/deployment.py
--rw-r--r--   0        0        0    14874 2022-04-18 09:52:35.271087 web3-ethereum-defi-0.8/eth_defi/uniswap_v2/fees.py
--rw-r--r--   0        0        0     2629 2022-05-06 09:56:03.435532 web3-ethereum-defi-0.8/eth_defi/uniswap_v2/liquidity.py
--rw-r--r--   0        0        0     5471 2022-05-12 13:58:10.428922 web3-ethereum-defi-0.8/eth_defi/uniswap_v2/swap.py
--rw-r--r--   0        0        0     9264 2022-05-06 12:01:57.116370 web3-ethereum-defi-0.8/eth_defi/uniswap_v2/token_tax.py
--rw-r--r--   0        0        0     1463 2022-04-18 09:52:19.039221 web3-ethereum-defi-0.8/eth_defi/uniswap_v2/utils.py
--rw-r--r--   0        0        0    99605 2022-04-04 18:53:58.121970 web3-ethereum-defi-0.8/eth_defi/uniswap_v3/constants.py
--rw-r--r--   0        0        0     9564 2022-04-18 08:58:35.684598 web3-ethereum-defi-0.8/eth_defi/uniswap_v3/deployment.py
--rw-r--r--   0        0        0     1702 2022-04-18 09:51:55.039403 web3-ethereum-defi-0.8/eth_defi/uniswap_v3/utils.py
--rw-r--r--   0        0        0      687 2022-04-18 09:49:54.296485 web3-ethereum-defi-0.8/eth_defi/utils.py
--rw-r--r--   0        0        0     1513 2022-05-12 13:57:41.355371 web3-ethereum-defi-0.8/pyproject.toml
--rw-r--r--   0        0        0    11585 2022-05-12 14:01:47.561945 web3-ethereum-defi-0.8/setup.py
--rw-r--r--   0        0        0    11384 2022-05-12 14:01:47.562356 web3-ethereum-defi-0.8/PKG-INFO
+-rw-r--r--   0        0        0     1059 2022-05-25 09:47:30.516467 web3-ethereum-defi-0.9/LICENSE.txt
+-rw-r--r--   0        0        0    10279 2022-05-25 09:47:30.516641 web3-ethereum-defi-0.9/README.md
+-rw-r--r--   0        0        0     6145 2022-05-25 09:47:30.519223 web3-ethereum-defi-0.9/eth_defi/abi/BaseBoringBatchable.json
+-rw-r--r--   0        0        0    97771 2022-05-25 09:47:30.519522 web3-ethereum-defi-0.9/eth_defi/abi/BentoBoxV1.json
+-rw-r--r--   0        0        0     8730 2022-05-25 09:47:30.519609 web3-ethereum-defi-0.9/eth_defi/abi/BoringBatchable.json
+-rw-r--r--   0        0        0      665 2022-05-25 09:47:30.519747 web3-ethereum-defi-0.9/eth_defi/abi/BoringERC20.json
+-rw-r--r--   0        0        0     5849 2022-05-25 09:47:30.519868 web3-ethereum-defi-0.9/eth_defi/abi/BoringFactory.json
+-rw-r--r--   0        0        0      664 2022-05-25 09:47:30.519934 web3-ethereum-defi-0.9/eth_defi/abi/BoringMath.json
+-rw-r--r--   0        0        0      667 2022-05-25 09:47:30.519984 web3-ethereum-defi-0.9/eth_defi/abi/BoringMath128.json
+-rw-r--r--   0        0        0      655 2022-05-25 09:47:30.520038 web3-ethereum-defi-0.9/eth_defi/abi/BoringMath32.json
+-rw-r--r--   0        0        0      655 2022-05-25 09:47:30.520096 web3-ethereum-defi-0.9/eth_defi/abi/BoringMath64.json
+-rw-r--r--   0        0        0     5657 2022-05-25 09:47:30.520229 web3-ethereum-defi-0.9/eth_defi/abi/BoringOwnable.json
+-rw-r--r--   0        0        0     1590 2022-05-25 09:47:30.520303 web3-ethereum-defi-0.9/eth_defi/abi/BoringOwnableData.json
+-rw-r--r--   0        0        0    37476 2022-05-25 09:47:30.520424 web3-ethereum-defi-0.9/eth_defi/abi/CloneRewarderTime.json
+-rw-r--r--   0        0        0    45593 2022-05-25 09:47:30.520574 web3-ethereum-defi-0.9/eth_defi/abi/CloneRewarderTimeDual.json
+-rw-r--r--   0        0        0    38288 2022-05-25 09:47:30.520714 web3-ethereum-defi-0.9/eth_defi/abi/ComplexRewarder.json
+-rw-r--r--   0        0        0    39055 2022-05-25 09:47:30.520793 web3-ethereum-defi-0.9/eth_defi/abi/ComplexRewarderTime.json
+-rw-r--r--   0        0        0     2394 2022-05-25 09:47:30.520902 web3-ethereum-defi-0.9/eth_defi/abi/Domain.json
+-rw-r--r--   0        0        0    16310 2022-05-25 09:47:30.521024 web3-ethereum-defi-0.9/eth_defi/abi/ERC20.json
+-rw-r--r--   0        0        0     3089 2022-05-25 09:47:30.521114 web3-ethereum-defi-0.9/eth_defi/abi/ERC20Data.json
+-rw-r--r--   0        0        0    18473 2022-05-25 09:47:30.521372 web3-ethereum-defi-0.9/eth_defi/abi/ERC20Mock.json
+-rw-r--r--   0        0        0    18679 2022-05-25 09:47:30.521476 web3-ethereum-defi-0.9/eth_defi/abi/ERC20MockDecimals.json
+-rw-r--r--   0        0        0     1002 2022-05-25 09:47:30.521563 web3-ethereum-defi-0.9/eth_defi/abi/IBatchFlashBorrower.json
+-rw-r--r--   0        0        0    24473 2022-05-25 09:47:30.521814 web3-ethereum-defi-0.9/eth_defi/abi/IBentoBoxV1.json
+-rw-r--r--   0        0        0     1204 2022-05-25 09:47:30.521931 web3-ethereum-defi-0.9/eth_defi/abi/IBentoBoxWithdraw.json
+-rw-r--r--   0        0        0     3831 2022-05-25 09:47:30.522026 web3-ethereum-defi-0.9/eth_defi/abi/IERC20.json
+-rw-r--r--   0        0        0     4737 2022-05-25 09:47:30.522111 web3-ethereum-defi-0.9/eth_defi/abi/IERC20Uniswap.json
+-rw-r--r--   0        0        0      977 2022-05-25 09:47:30.522167 web3-ethereum-defi-0.9/eth_defi/abi/IFlashBorrower.json
+-rw-r--r--   0        0        0     1513 2022-05-25 09:47:30.522235 web3-ethereum-defi-0.9/eth_defi/abi/IKashiWithdrawFee.json
+-rw-r--r--   0        0        0     1873 2022-05-25 09:47:30.522348 web3-ethereum-defi-0.9/eth_defi/abi/IMasterChef.json
+-rw-r--r--   0        0        0      636 2022-05-25 09:47:30.522406 web3-ethereum-defi-0.9/eth_defi/abi/IMasterChefV2.json
+-rw-r--r--   0        0        0      508 2022-05-25 09:47:30.522460 web3-ethereum-defi-0.9/eth_defi/abi/IMasterContract.json
+-rw-r--r--   0        0        0      504 2022-05-25 09:47:30.522523 web3-ethereum-defi-0.9/eth_defi/abi/IMigrator.json
+-rw-r--r--   0        0        0      627 2022-05-25 09:47:30.522575 web3-ethereum-defi-0.9/eth_defi/abi/IMigratorChef.json
+-rw-r--r--   0        0        0     4157 2022-05-25 09:47:30.522737 web3-ethereum-defi-0.9/eth_defi/abi/IMiniChefV2.json
+-rw-r--r--   0        0        0     2296 2022-05-25 09:47:30.522841 web3-ethereum-defi-0.9/eth_defi/abi/IOracle.json
+-rw-r--r--   0        0        0     1703 2022-05-25 09:47:30.522962 web3-ethereum-defi-0.9/eth_defi/abi/IRewarder.json
+-rw-r--r--   0        0        0     1786 2022-05-25 09:47:30.523040 web3-ethereum-defi-0.9/eth_defi/abi/IStrategy.json
+-rw-r--r--   0        0        0     2362 2022-05-25 09:47:30.523112 web3-ethereum-defi-0.9/eth_defi/abi/ISwapper.json
+-rw-r--r--   0        0        0      872 2022-05-25 09:47:30.523201 web3-ethereum-defi-0.9/eth_defi/abi/IUniswapV2Callee.json
+-rw-r--r--   0        0        0     6564 2022-05-25 09:47:30.523280 web3-ethereum-defi-0.9/eth_defi/abi/IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     4095 2022-05-25 09:47:30.523342 web3-ethereum-defi-0.9/eth_defi/abi/IUniswapV2Factory.json
+-rw-r--r--   0        0        0    13664 2022-05-25 09:47:30.523395 web3-ethereum-defi-0.9/eth_defi/abi/IUniswapV2Pair.json
+-rw-r--r--   0        0        0    16744 2022-05-25 09:47:30.523585 web3-ethereum-defi-0.9/eth_defi/abi/IUniswapV2Router01.json
+-rw-r--r--   0        0        0    21403 2022-05-25 09:47:30.523659 web3-ethereum-defi-0.9/eth_defi/abi/IUniswapV2Router02.json
+-rw-r--r--   0        0        0      634 2022-05-25 09:47:30.523719 web3-ethereum-defi-0.9/eth_defi/abi/IWETH.json
+-rw-r--r--   0        0        0   122472 2022-05-25 09:47:30.524065 web3-ethereum-defi-0.9/eth_defi/abi/KashiPairMediumRiskV1.json
+-rw-r--r--   0        0        0     3162 2022-05-25 09:47:30.524140 web3-ethereum-defi-0.9/eth_defi/abi/MalformedERC20.json
+-rw-r--r--   0        0        0    41078 2022-05-25 09:47:30.524210 web3-ethereum-defi-0.9/eth_defi/abi/MasterChef.json
+-rw-r--r--   0        0        0    68638 2022-05-25 09:47:30.524310 web3-ethereum-defi-0.9/eth_defi/abi/MasterChefV2.json
+-rw-r--r--   0        0        0    25138 2022-05-25 09:47:30.524381 web3-ethereum-defi-0.9/eth_defi/abi/MasterContractManager.json
+-rw-r--r--   0        0        0      652 2022-05-25 09:47:30.524454 web3-ethereum-defi-0.9/eth_defi/abi/Math.json
+-rw-r--r--   0        0        0     9753 2022-05-25 09:47:30.524501 web3-ethereum-defi-0.9/eth_defi/abi/Migrator.json
+-rw-r--r--   0        0        0    64126 2022-05-25 09:47:30.524646 web3-ethereum-defi-0.9/eth_defi/abi/MiniChefV2.json
+-rw-r--r--   0        0        0    16797 2022-05-25 09:47:30.524737 web3-ethereum-defi-0.9/eth_defi/abi/Multicall2.json
+-rw-r--r--   0        0        0     1790 2022-05-25 09:47:30.524801 web3-ethereum-defi-0.9/eth_defi/abi/Ownable.json
+-rw-r--r--   0        0        0     1511 2022-05-25 09:47:30.524872 web3-ethereum-defi-0.9/eth_defi/abi/OwnableData.json
+-rw-r--r--   0        0        0     6464 2022-05-25 09:47:30.524942 web3-ethereum-defi-0.9/eth_defi/abi/PeggedOracleV1.json
+-rw-r--r--   0        0        0      667 2022-05-25 09:47:30.524995 web3-ethereum-defi-0.9/eth_defi/abi/RebaseLibrary.json
+-rw-r--r--   0        0        0     3335 2022-05-25 09:47:30.525067 web3-ethereum-defi-0.9/eth_defi/abi/RewarderBrokenMock.json
+-rw-r--r--   0        0        0     8849 2022-05-25 09:47:30.525118 web3-ethereum-defi-0.9/eth_defi/abi/RewarderMock.json
+-rw-r--r--   0        0        0     2454 2022-05-25 09:47:30.525179 web3-ethereum-defi-0.9/eth_defi/abi/SafeERC20.json
+-rw-r--r--   0        0        0      650 2022-05-25 09:47:30.525231 web3-ethereum-defi-0.9/eth_defi/abi/SafeMath.json
+-rw-r--r--   0        0        0      653 2022-05-25 09:47:30.525278 web3-ethereum-defi-0.9/eth_defi/abi/SafeMath128.json
+-rw-r--r--   0        0        0      667 2022-05-25 09:47:30.525328 web3-ethereum-defi-0.9/eth_defi/abi/SafeMathUniswap.json
+-rw-r--r--   0        0        0      662 2022-05-25 09:47:30.525379 web3-ethereum-defi-0.9/eth_defi/abi/SignedSafeMath.json
+-rw-r--r--   0        0        0    24381 2022-05-25 09:47:30.525480 web3-ethereum-defi-0.9/eth_defi/abi/SushiBar.json
+-rw-r--r--   0        0        0    29251 2022-05-25 09:47:30.525589 web3-ethereum-defi-0.9/eth_defi/abi/SushiMaker.json
+-rw-r--r--   0        0        0     2896 2022-05-25 09:47:30.525659 web3-ethereum-defi-0.9/eth_defi/abi/SushiMakerExploitMock.json
+-rw-r--r--   0        0        0    21943 2022-05-25 09:47:30.525746 web3-ethereum-defi-0.9/eth_defi/abi/SushiMakerKashi.json
+-rw-r--r--   0        0        0     2715 2022-05-25 09:47:30.525823 web3-ethereum-defi-0.9/eth_defi/abi/SushiMakerKashiExploitMock.json
+-rw-r--r--   0        0        0    20673 2022-05-25 09:47:30.525907 web3-ethereum-defi-0.9/eth_defi/abi/SushiRoll.json
+-rw-r--r--   0        0        0    49829 2022-05-25 09:47:30.525994 web3-ethereum-defi-0.9/eth_defi/abi/SushiSwapFactoryMock.json
+-rw-r--r--   0        0        0    50610 2022-05-25 09:47:30.526083 web3-ethereum-defi-0.9/eth_defi/abi/SushiSwapPairMock.json
+-rw-r--r--   0        0        0    41108 2022-05-25 09:47:30.526249 web3-ethereum-defi-0.9/eth_defi/abi/SushiToken.json
+-rw-r--r--   0        0        0    34840 2022-05-25 09:47:30.526364 web3-ethereum-defi-0.9/eth_defi/abi/Timelock.json
+-rw-r--r--   0        0        0      672 2022-05-25 09:47:30.526428 web3-ethereum-defi-0.9/eth_defi/abi/TransferHelper.json
+-rw-r--r--   0        0        0      662 2022-05-25 09:47:30.526479 web3-ethereum-defi-0.9/eth_defi/abi/UQ112x112.json
+-rw-r--r--   0        0        0    15775 2022-05-25 09:47:30.526532 web3-ethereum-defi-0.9/eth_defi/abi/UniswapV2ERC20.json
+-rw-r--r--   0        0        0    49825 2022-05-25 09:47:30.526611 web3-ethereum-defi-0.9/eth_defi/abi/UniswapV2Factory.json
+-rw-r--r--   0        0        0      676 2022-05-25 09:47:30.526679 web3-ethereum-defi-0.9/eth_defi/abi/UniswapV2Library.json
+-rw-r--r--   0        0        0    50606 2022-05-25 09:47:30.526751 web3-ethereum-defi-0.9/eth_defi/abi/UniswapV2Pair.json
+-rw-r--r--   0        0        0    93624 2022-05-25 09:47:30.526857 web3-ethereum-defi-0.9/eth_defi/abi/UniswapV2Router02.json
+-rw-r--r--   0        0        0    14171 2022-05-25 09:47:30.526952 web3-ethereum-defi-0.9/eth_defi/abi/WETH9Mock.json
+-rw-r--r--   0        0        0     5423 2022-05-25 09:47:30.527256 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/Base64Test.json
+-rw-r--r--   0        0        0      484 2022-05-25 09:47:30.527319 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/BitMath.json
+-rw-r--r--   0        0        0     3518 2022-05-25 09:47:30.527397 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/BitMathEchidnaTest.json
+-rw-r--r--   0        0        0     4755 2022-05-25 09:47:30.527476 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/BitMathTest.json
+-rw-r--r--   0        0        0      243 2022-05-25 09:47:30.527529 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/BlockTimestamp.json
+-rw-r--r--   0        0        0      486 2022-05-25 09:47:30.527579 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/BytesLib.json
+-rw-r--r--   0        0        0      506 2022-05-25 09:47:30.527625 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/CallbackValidation.json
+-rw-r--r--   0        0        0      484 2022-05-25 09:47:30.527672 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/ChainId.json
+-rw-r--r--   0        0        0     9758 2022-05-25 09:47:30.527742 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/ERC721Permit.json
+-rw-r--r--   0        0        0      496 2022-05-25 09:47:30.527799 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/FixedPoint128.json
+-rw-r--r--   0        0        0      494 2022-05-25 09:47:30.527847 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/FixedPoint96.json
+-rw-r--r--   0        0        0      486 2022-05-25 09:47:30.527901 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/FullMath.json
+-rw-r--r--   0        0        0     4959 2022-05-25 09:47:30.528035 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/FullMathEchidnaTest.json
+-rw-r--r--   0        0        0     3245 2022-05-25 09:47:30.528097 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/FullMathTest.json
+-rw-r--r--   0        0        0      490 2022-05-25 09:47:30.528147 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/HexStrings.json
+-rw-r--r--   0        0        0      747 2022-05-25 09:47:30.528198 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IERC1271.json
+-rw-r--r--   0        0        0     4757 2022-05-25 09:47:30.528298 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IERC20Metadata.json
+-rw-r--r--   0        0        0     3758 2022-05-25 09:47:30.528594 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IERC20Minimal.json
+-rw-r--r--   0        0        0     1306 2022-05-25 09:47:30.528649 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IERC20PermitAllowed.json
+-rw-r--r--   0        0        0     7547 2022-05-25 09:47:30.528715 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IERC721Permit.json
+-rw-r--r--   0        0        0      624 2022-05-25 09:47:30.528784 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IMulticall.json
+-rw-r--r--   0        0        0    22092 2022-05-25 09:47:30.529096 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/INonfungiblePositionManager.json
+-rw-r--r--   0        0        0     1228 2022-05-25 09:47:30.529231 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/INonfungibleTokenPositionDescriptor.json
+-rw-r--r--   0        0        0      771 2022-05-25 09:47:30.529301 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IPeripheryImmutableState.json
+-rw-r--r--   0        0        0     1289 2022-05-25 09:47:30.529610 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IPeripheryPayments.json
+-rw-r--r--   0        0        0     2675 2022-05-25 09:47:30.529683 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IPeripheryPaymentsWithFee.json
+-rw-r--r--   0        0        0     1003 2022-05-25 09:47:30.529742 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IPoolInitializer.json
+-rw-r--r--   0        0        0     2981 2022-05-25 09:47:30.529918 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IQuoter.json
+-rw-r--r--   0        0        0     5081 2022-05-25 09:47:30.529977 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IQuoterV2.json
+-rw-r--r--   0        0        0     3533 2022-05-25 09:47:30.530049 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/ISelfPermit.json
+-rw-r--r--   0        0        0     6136 2022-05-25 09:47:30.530102 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/ISwapRouter.json
+-rw-r--r--   0        0        0     1230 2022-05-25 09:47:30.530204 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/ITickLens.json
+-rw-r--r--   0        0        0     4350 2022-05-25 09:47:30.530254 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3Factory.json
+-rw-r--r--   0        0        0      774 2022-05-25 09:47:30.530313 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3FlashCallback.json
+-rw-r--r--   0        0        0      785 2022-05-25 09:47:30.530367 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3MintCallback.json
+-rw-r--r--   0        0        0    21755 2022-05-25 09:47:30.530423 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3Pool.json
+-rw-r--r--   0        0        0     5058 2022-05-25 09:47:30.530492 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolActions.json
+-rw-r--r--   0        0        0      980 2022-05-25 09:47:30.530550 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolDeployer.json
+-rw-r--r--   0        0        0     1592 2022-05-25 09:47:30.530605 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolDerivedState.json
+-rw-r--r--   0        0        0     7617 2022-05-25 09:47:30.530671 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolEvents.json
+-rw-r--r--   0        0        0     1786 2022-05-25 09:47:30.530727 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolImmutables.json
+-rw-r--r--   0        0        0     1426 2022-05-25 09:47:30.530811 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolOwnerActions.json
+-rw-r--r--   0        0        0     5665 2022-05-25 09:47:30.530869 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolState.json
+-rw-r--r--   0        0        0      783 2022-05-25 09:47:30.530924 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3SwapCallback.json
+-rw-r--r--   0        0        0     6752 2022-05-25 09:47:30.530978 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IV3Migrator.json
+-rw-r--r--   0        0        0     4406 2022-05-25 09:47:30.531032 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IWETH9.json
+-rw-r--r--   0        0        0      502 2022-05-25 09:47:30.531102 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/LiquidityAmounts.json
+-rw-r--r--   0        0        0    20362 2022-05-25 09:47:30.531195 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/LiquidityAmountsTest.json
+-rw-r--r--   0        0        0     2367 2022-05-25 09:47:30.531269 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/LiquidityManagement.json
+-rw-r--r--   0        0        0      496 2022-05-25 09:47:30.531322 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/LiquidityMath.json
+-rw-r--r--   0        0        0     3044 2022-05-25 09:47:30.531381 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/LiquidityMathTest.json
+-rw-r--r--   0        0        0      498 2022-05-25 09:47:30.531439 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/LowGasSafeMath.json
+-rw-r--r--   0        0        0     4807 2022-05-25 09:47:30.531507 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/LowGasSafeMathEchidnaTest.json
+-rw-r--r--   0        0        0     6854 2022-05-25 09:47:30.531579 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/MockObservable.json
+-rw-r--r--   0        0        0     7231 2022-05-25 09:47:30.531627 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/MockObservations.json
+-rw-r--r--   0        0        0   126981 2022-05-25 09:47:30.531738 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/MockTimeNonfungiblePositionManager.json
+-rw-r--r--   0        0        0    62557 2022-05-25 09:47:30.531832 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/MockTimeSwapRouter.json
+-rw-r--r--   0        0        0   113293 2022-05-25 09:47:30.531947 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/MockTimeUniswapV3Pool.json
+-rw-r--r--   0        0        0    97190 2022-05-25 09:47:30.532286 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/MockTimeUniswapV3PoolDeployer.json
+-rw-r--r--   0        0        0      616 2022-05-25 09:47:30.532360 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/Multicall.json
+-rw-r--r--   0        0        0   100849 2022-05-25 09:47:30.532674 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NFTDescriptor.json
+-rw-r--r--   0        0        0   108664 2022-05-25 09:47:30.532792 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NFTDescriptorTest.json
+-rw-r--r--   0        0        0      482 2022-05-25 09:47:30.532856 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NFTSVG.json
+-rw-r--r--   0        0        0      238 2022-05-25 09:47:30.532914 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NoDelegateCall.json
+-rw-r--r--   0        0        0     2906 2022-05-25 09:47:30.533001 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NoDelegateCallTest.json
+-rw-r--r--   0        0        0   126423 2022-05-25 09:47:30.533206 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NonfungiblePositionManager.json
+-rw-r--r--   0        0        0     2289 2022-05-25 09:47:30.533538 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NonfungiblePositionManagerPositionsGasTest.json
+-rw-r--r--   0        0        0    22530 2022-05-25 09:47:30.533632 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NonfungibleTokenPositionDescriptor.json
+-rw-r--r--   0        0        0      482 2022-05-25 09:47:30.533703 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/Oracle.json
+-rw-r--r--   0        0        0    32780 2022-05-25 09:47:30.533854 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/OracleEchidnaTest.json
+-rw-r--r--   0        0        0      496 2022-05-25 09:47:30.533930 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/OracleLibrary.json
+-rw-r--r--   0        0        0    28516 2022-05-25 09:47:30.534035 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/OracleTest.json
+-rw-r--r--   0        0        0    30909 2022-05-25 09:47:30.534163 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PairFlash.json
+-rw-r--r--   0        0        0      478 2022-05-25 09:47:30.534229 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/Path.json
+-rw-r--r--   0        0        0    11849 2022-05-25 09:47:30.534299 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PathTest.json
+-rw-r--r--   0        0        0      763 2022-05-25 09:47:30.534361 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PeripheryImmutableState.json
+-rw-r--r--   0        0        0     2123 2022-05-25 09:47:30.534452 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PeripheryImmutableStateTest.json
+-rw-r--r--   0        0        0     1854 2022-05-25 09:47:30.534515 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PeripheryPayments.json
+-rw-r--r--   0        0        0     3240 2022-05-25 09:47:30.534590 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PeripheryPaymentsWithFee.json
+-rw-r--r--   0        0        0      253 2022-05-25 09:47:30.534653 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PeripheryValidation.json
+-rw-r--r--   0        0        0      492 2022-05-25 09:47:30.534715 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PoolAddress.json
+-rw-r--r--   0        0        0     5434 2022-05-25 09:47:30.534815 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PoolAddressTest.json
+-rw-r--r--   0        0        0     1495 2022-05-25 09:47:30.534874 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PoolInitializer.json
+-rw-r--r--   0        0        0      502 2022-05-25 09:47:30.534929 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PoolTicksCounter.json
+-rw-r--r--   0        0        0     8519 2022-05-25 09:47:30.535010 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PoolTicksCounterTest.json
+-rw-r--r--   0        0        0      486 2022-05-25 09:47:30.535098 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/Position.json
+-rw-r--r--   0        0        0      492 2022-05-25 09:47:30.535160 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PositionKey.json
+-rw-r--r--   0        0        0      496 2022-05-25 09:47:30.535228 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PositionValue.json
+-rw-r--r--   0        0        0    22712 2022-05-25 09:47:30.535305 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PositionValueTest.json
+-rw-r--r--   0        0        0    23246 2022-05-25 09:47:30.535427 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/Quoter.json
+-rw-r--r--   0        0        0    39940 2022-05-25 09:47:30.535565 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/QuoterV2.json
+-rw-r--r--   0        0        0      486 2022-05-25 09:47:30.535625 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SafeCast.json
+-rw-r--r--   0        0        0     3525 2022-05-25 09:47:30.535675 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SelfPermit.json
+-rw-r--r--   0        0        0     8241 2022-05-25 09:47:30.535742 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SelfPermitTest.json
+-rw-r--r--   0        0        0      496 2022-05-25 09:47:30.535791 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SqrtPriceMath.json
+-rw-r--r--   0        0        0    23360 2022-05-25 09:47:30.535858 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SqrtPriceMathEchidnaTest.json
+-rw-r--r--   0        0        0      510 2022-05-25 09:47:30.535932 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SqrtPriceMathPartial.json
+-rw-r--r--   0        0        0    14691 2022-05-25 09:47:30.535991 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SqrtPriceMathTest.json
+-rw-r--r--   0        0        0      486 2022-05-25 09:47:30.536045 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SwapMath.json
+-rw-r--r--   0        0        0    10378 2022-05-25 09:47:30.536124 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SwapMathEchidnaTest.json
+-rw-r--r--   0        0        0    10768 2022-05-25 09:47:30.536173 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SwapMathTest.json
+-rw-r--r--   0        0        0    61914 2022-05-25 09:47:30.536259 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SwapRouter.json
+-rw-r--r--   0        0        0     4049 2022-05-25 09:47:30.536338 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestCallbackValidation.json
+-rw-r--r--   0        0        0    29157 2022-05-25 09:47:30.536393 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestERC20.json
+-rw-r--r--   0        0        0    29989 2022-05-25 09:47:30.536490 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestERC20Metadata.json
+-rw-r--r--   0        0        0    32063 2022-05-25 09:47:30.536584 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestERC20PermitAllowed.json
+-rw-r--r--   0        0        0     9382 2022-05-25 09:47:30.536660 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestMulticall.json
+-rw-r--r--   0        0        0     4429 2022-05-25 09:47:30.536729 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestPositionNFTOwner.json
+-rw-r--r--   0        0        0    11052 2022-05-25 09:47:30.536800 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestUniswapV3Callee.json
+-rw-r--r--   0        0        0    16971 2022-05-25 09:47:30.536877 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestUniswapV3ReentrantCallee.json
+-rw-r--r--   0        0        0    12791 2022-05-25 09:47:30.536941 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestUniswapV3Router.json
+-rw-r--r--   0        0        0     6352 2022-05-25 09:47:30.536988 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestUniswapV3SwapPay.json
+-rw-r--r--   0        0        0      478 2022-05-25 09:47:30.537041 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/Tick.json
+-rw-r--r--   0        0        0      490 2022-05-25 09:47:30.537099 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickBitmap.json
+-rw-r--r--   0        0        0     6473 2022-05-25 09:47:30.537157 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickBitmapEchidnaTest.json
+-rw-r--r--   0        0        0     8559 2022-05-25 09:47:30.537212 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickBitmapTest.json
+-rw-r--r--   0        0        0     2392 2022-05-25 09:47:30.537405 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickEchidnaTest.json
+-rw-r--r--   0        0        0     6826 2022-05-25 09:47:30.537548 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickLens.json
+-rw-r--r--   0        0        0     7666 2022-05-25 09:47:30.537603 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickLensTest.json
+-rw-r--r--   0        0        0      486 2022-05-25 09:47:30.537658 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickMath.json
+-rw-r--r--   0        0        0     9186 2022-05-25 09:47:30.537736 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickMathEchidnaTest.json
+-rw-r--r--   0        0        0    10809 2022-05-25 09:47:30.537816 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickMathTest.json
+-rw-r--r--   0        0        0    10086 2022-05-25 09:47:30.537896 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickOverflowSafetyEchidnaTest.json
+-rw-r--r--   0        0        0    19533 2022-05-25 09:47:30.537993 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickTest.json
+-rw-r--r--   0        0        0      508 2022-05-25 09:47:30.538081 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TokenRatioSortOrder.json
+-rw-r--r--   0        0        0      498 2022-05-25 09:47:30.538138 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TransferHelper.json
+-rw-r--r--   0        0        0     7971 2022-05-25 09:47:30.538214 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/UniswapInterfaceMulticall.json
+-rw-r--r--   0        0        0   104076 2022-05-25 09:47:30.538335 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/UniswapV3Factory.json
+-rw-r--r--   0        0        0   111557 2022-05-25 09:47:30.538572 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/UniswapV3Pool.json
+-rw-r--r--   0        0        0     2017 2022-05-25 09:47:30.538650 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/UniswapV3PoolDeployer.json
+-rw-r--r--   0        0        0     6910 2022-05-25 09:47:30.538724 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/UniswapV3PoolSwapTest.json
+-rw-r--r--   0        0        0      490 2022-05-25 09:47:30.538771 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/UnsafeMath.json
+-rw-r--r--   0        0        0     1413 2022-05-25 09:47:30.538845 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/UnsafeMathEchidnaTest.json
+-rw-r--r--   0        0        0    39457 2022-05-25 09:47:30.538965 web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/V3Migrator.json
+-rw-r--r--   0        0        0     3383 2022-05-25 09:47:30.519101 web3-ethereum-defi-0.9/eth_defi/abi.py
+-rw-r--r--   0        0        0     6518 2022-05-25 09:47:30.539070 web3-ethereum-defi-0.9/eth_defi/balances.py
+-rw-r--r--   0        0        0     8620 2022-05-30 17:31:46.021252 web3-ethereum-defi-0.9/eth_defi/confirmation.py
+-rw-r--r--   0        0        0     1319 2022-05-25 09:47:30.539134 web3-ethereum-defi-0.9/eth_defi/deploy.py
+-rw-r--r--   0        0        0     3470 2022-05-25 09:47:30.539204 web3-ethereum-defi-0.9/eth_defi/event.py
+-rw-r--r--   0        0        0     2132 2022-05-25 09:47:30.539298 web3-ethereum-defi-0.9/eth_defi/event_reader/conversion.py
+-rw-r--r--   0        0        0     1421 2022-05-25 09:47:30.539373 web3-ethereum-defi-0.9/eth_defi/event_reader/fast_json_rpc.py
+-rw-r--r--   0        0        0     1369 2022-05-25 09:47:30.539442 web3-ethereum-defi-0.9/eth_defi/event_reader/logresult.py
+-rw-r--r--   0        0        0    15165 2022-05-25 09:47:30.539537 web3-ethereum-defi-0.9/eth_defi/event_reader/reader.py
+-rw-r--r--   0        0        0     1369 2022-05-25 09:47:30.539600 web3-ethereum-defi-0.9/eth_defi/event_reader/web3factory.py
+-rw-r--r--   0        0        0     1056 2022-05-25 09:47:30.539666 web3-ethereum-defi-0.9/eth_defi/event_reader/web3worker.py
+-rw-r--r--   0        0        0    15843 2022-05-25 13:53:25.929410 web3-ethereum-defi-0.9/eth_defi/ganache.py
+-rw-r--r--   0        0        0     4434 2022-05-26 18:52:46.007182 web3-ethereum-defi-0.9/eth_defi/gas.py
+-rw-r--r--   0        0        0     3753 2022-05-30 18:02:36.247874 web3-ethereum-defi-0.9/eth_defi/hotwallet.py
+-rw-r--r--   0        0        0     3002 2022-05-25 09:47:30.539993 web3-ethereum-defi-0.9/eth_defi/middleware.py
+-rw-r--r--   0        0        0     5190 2022-05-25 09:47:30.540076 web3-ethereum-defi-0.9/eth_defi/revert_reason.py
+-rw-r--r--   0        0        0     6544 2022-05-25 09:47:30.540166 web3-ethereum-defi-0.9/eth_defi/token.py
+-rw-r--r--   0        0        0     2367 2022-05-30 18:39:28.049474 web3-ethereum-defi-0.9/eth_defi/tx.py
+-rw-r--r--   0        0        0     8082 2022-05-30 18:44:51.971407 web3-ethereum-defi-0.9/eth_defi/uniswap_v2/analysis.py
+-rw-r--r--   0        0        0    57469 2022-05-25 09:47:30.540639 web3-ethereum-defi-0.9/eth_defi/uniswap_v2/deployment.py
+-rw-r--r--   0        0        0    19311 2022-05-25 09:47:30.540753 web3-ethereum-defi-0.9/eth_defi/uniswap_v2/fees.py
+-rw-r--r--   0        0        0     2621 2022-05-25 09:47:30.540827 web3-ethereum-defi-0.9/eth_defi/uniswap_v2/liquidity.py
+-rw-r--r--   0        0        0     5471 2022-05-25 09:47:30.540912 web3-ethereum-defi-0.9/eth_defi/uniswap_v2/swap.py
+-rw-r--r--   0        0        0     9270 2022-05-25 09:47:30.540996 web3-ethereum-defi-0.9/eth_defi/uniswap_v2/token_tax.py
+-rw-r--r--   0        0        0     1603 2022-05-25 09:47:30.541068 web3-ethereum-defi-0.9/eth_defi/uniswap_v2/utils.py
+-rw-r--r--   0        0        0    99605 2022-05-25 09:47:30.541454 web3-ethereum-defi-0.9/eth_defi/uniswap_v3/constants.py
+-rw-r--r--   0        0        0     9564 2022-05-25 09:47:30.541578 web3-ethereum-defi-0.9/eth_defi/uniswap_v3/deployment.py
+-rw-r--r--   0        0        0     1702 2022-05-25 09:47:30.541643 web3-ethereum-defi-0.9/eth_defi/uniswap_v3/utils.py
+-rw-r--r--   0        0        0      687 2022-05-25 09:47:30.541701 web3-ethereum-defi-0.9/eth_defi/utils.py
+-rw-r--r--   0        0        0     1593 2022-06-01 16:10:28.380083 web3-ethereum-defi-0.9/pyproject.toml
+-rw-r--r--   0        0        0    11796 2022-06-01 16:10:59.611694 web3-ethereum-defi-0.9/setup.py
+-rw-r--r--   0        0        0    11607 2022-06-01 16:10:59.612094 web3-ethereum-defi-0.9/PKG-INFO
```

### Comparing `web3-ethereum-defi-0.8/LICENSE.txt` & `web3-ethereum-defi-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/README.md` & `web3-ethereum-defi-0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
    * [Uniswap v2 trade example](#uniswap-v2-trade-example)
    * [Uniswap v2 price estimation example](#uniswap-v2-price-estimation-example)
    * [How to use the library in your Python project](#how-to-use-the-library-in-your-python-project)
 * [Development](#development)
    * [Build requirements](#build-requirements)
    * [Make](#make)
 * [Version history](#version-history)
-* [Discord](#discord)
+* [Social media](#social-media)
 * [Notes](#notes)
 * [History](#history)
 * [License](#license)
 
 ![Pepe chooses Web3 Ethereum DeFi and Python](https://raw.githubusercontent.com/tradingstrategy-ai/web3-ethereum-defi/master/docs/source/_static/pepe.jpg)
 
 **Pepe chooses web3-ethereum-defi and Python**.
@@ -250,17 +250,18 @@
 [Read development instructions](https://web3-ethereum-defi.readthedocs.io/development.html).
 
 # Version history
 
 - [Read changelog](https://github.com/tradingstrategy-ai/web3-ethereum-defi/blob/master/CHANGELOG.md).
 - [See releases](https://pypi.org/project/web3-ethereum-defi/#history).
 
-# Discord
+# Social media
 
-[Join Discord for any questions](https://tradingstrategy.ai/community).
+- [Join Discord for any questions](https://tradingstrategy.ai/community).
+- [Message us on Twitter](https://twitter.com/TradingProtocol)
 
 # Notes
 
 Currently there is no [Brownie](https://eth-brownie.readthedocs.io/) support.
 To support Brownie, one would need to figure out how to import an existing Hardhat
 based project (Sushiswap) to Brownie project format.
```

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/BaseBoringBatchable.json` & `web3-ethereum-defi-0.9/eth_defi/abi/BaseBoringBatchable.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/BentoBoxV1.json` & `web3-ethereum-defi-0.9/eth_defi/abi/BentoBoxV1.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/BoringBatchable.json` & `web3-ethereum-defi-0.9/eth_defi/abi/BoringBatchable.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/BoringERC20.json` & `web3-ethereum-defi-0.9/eth_defi/abi/BoringERC20.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/BoringFactory.json` & `web3-ethereum-defi-0.9/eth_defi/abi/BoringFactory.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/BoringMath.json` & `web3-ethereum-defi-0.9/eth_defi/abi/BoringMath.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/BoringMath128.json` & `web3-ethereum-defi-0.9/eth_defi/abi/BoringMath128.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/BoringMath32.json` & `web3-ethereum-defi-0.9/eth_defi/abi/BoringMath32.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/BoringMath64.json` & `web3-ethereum-defi-0.9/eth_defi/abi/BoringMath64.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/BoringOwnable.json` & `web3-ethereum-defi-0.9/eth_defi/abi/BoringOwnable.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/BoringOwnableData.json` & `web3-ethereum-defi-0.9/eth_defi/abi/BoringOwnableData.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/CloneRewarderTime.json` & `web3-ethereum-defi-0.9/eth_defi/abi/CloneRewarderTime.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/CloneRewarderTimeDual.json` & `web3-ethereum-defi-0.9/eth_defi/abi/CloneRewarderTimeDual.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/ComplexRewarder.json` & `web3-ethereum-defi-0.9/eth_defi/abi/ComplexRewarder.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/ComplexRewarderTime.json` & `web3-ethereum-defi-0.9/eth_defi/abi/ComplexRewarderTime.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/Domain.json` & `web3-ethereum-defi-0.9/eth_defi/abi/Domain.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/ERC20.json` & `web3-ethereum-defi-0.9/eth_defi/abi/ERC20.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/ERC20Data.json` & `web3-ethereum-defi-0.9/eth_defi/abi/ERC20Data.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/ERC20Mock.json` & `web3-ethereum-defi-0.9/eth_defi/abi/ERC20Mock.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/ERC20MockDecimals.json` & `web3-ethereum-defi-0.9/eth_defi/abi/ERC20MockDecimals.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IBatchFlashBorrower.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IBatchFlashBorrower.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IBentoBoxV1.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IBentoBoxV1.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IBentoBoxWithdraw.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IBentoBoxWithdraw.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IERC20.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IERC20.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IERC20Uniswap.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IERC20Uniswap.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IFlashBorrower.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IFlashBorrower.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IKashiWithdrawFee.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IKashiWithdrawFee.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IMasterChef.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IMasterChef.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IMasterChefV2.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IMasterChefV2.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IMigratorChef.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IMigratorChef.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IMiniChefV2.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IMiniChefV2.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IOracle.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IOracle.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IRewarder.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IRewarder.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IStrategy.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IStrategy.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/ISwapper.json` & `web3-ethereum-defi-0.9/eth_defi/abi/ISwapper.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IUniswapV2Callee.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IUniswapV2Callee.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IUniswapV2ERC20.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IUniswapV2Factory.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IUniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IUniswapV2Pair.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IUniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IUniswapV2Router01.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IUniswapV2Router01.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IUniswapV2Router02.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IUniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/IWETH.json` & `web3-ethereum-defi-0.9/eth_defi/abi/IWETH.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/KashiPairMediumRiskV1.json` & `web3-ethereum-defi-0.9/eth_defi/abi/KashiPairMediumRiskV1.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/MalformedERC20.json` & `web3-ethereum-defi-0.9/eth_defi/abi/MalformedERC20.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/MasterChef.json` & `web3-ethereum-defi-0.9/eth_defi/abi/MasterChef.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/MasterChefV2.json` & `web3-ethereum-defi-0.9/eth_defi/abi/MasterChefV2.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/MasterContractManager.json` & `web3-ethereum-defi-0.9/eth_defi/abi/MasterContractManager.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/Math.json` & `web3-ethereum-defi-0.9/eth_defi/abi/Math.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/Migrator.json` & `web3-ethereum-defi-0.9/eth_defi/abi/Migrator.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/MiniChefV2.json` & `web3-ethereum-defi-0.9/eth_defi/abi/MiniChefV2.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/Multicall2.json` & `web3-ethereum-defi-0.9/eth_defi/abi/Multicall2.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/Ownable.json` & `web3-ethereum-defi-0.9/eth_defi/abi/Ownable.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/OwnableData.json` & `web3-ethereum-defi-0.9/eth_defi/abi/OwnableData.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/PeggedOracleV1.json` & `web3-ethereum-defi-0.9/eth_defi/abi/PeggedOracleV1.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/RebaseLibrary.json` & `web3-ethereum-defi-0.9/eth_defi/abi/RebaseLibrary.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/RewarderBrokenMock.json` & `web3-ethereum-defi-0.9/eth_defi/abi/RewarderBrokenMock.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/RewarderMock.json` & `web3-ethereum-defi-0.9/eth_defi/abi/RewarderMock.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SafeERC20.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SafeERC20.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SafeMath.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SafeMath128.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SafeMath128.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SafeMathUniswap.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SafeMathUniswap.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SignedSafeMath.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SignedSafeMath.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SushiBar.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SushiBar.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SushiMaker.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SushiMaker.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SushiMakerExploitMock.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SushiMakerExploitMock.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SushiMakerKashi.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SushiMakerKashi.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SushiMakerKashiExploitMock.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SushiMakerKashiExploitMock.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SushiRoll.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SushiRoll.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SushiSwapFactoryMock.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SushiSwapFactoryMock.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SushiSwapPairMock.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SushiSwapPairMock.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/SushiToken.json` & `web3-ethereum-defi-0.9/eth_defi/abi/SushiToken.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/Timelock.json` & `web3-ethereum-defi-0.9/eth_defi/abi/Timelock.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/TransferHelper.json` & `web3-ethereum-defi-0.9/eth_defi/abi/TransferHelper.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/UQ112x112.json` & `web3-ethereum-defi-0.9/eth_defi/abi/UQ112x112.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/UniswapV2ERC20.json` & `web3-ethereum-defi-0.9/eth_defi/abi/UniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/UniswapV2Factory.json` & `web3-ethereum-defi-0.9/eth_defi/abi/UniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/UniswapV2Library.json` & `web3-ethereum-defi-0.9/eth_defi/abi/UniswapV2Library.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/UniswapV2Pair.json` & `web3-ethereum-defi-0.9/eth_defi/abi/UniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/UniswapV2Router02.json` & `web3-ethereum-defi-0.9/eth_defi/abi/UniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/WETH9Mock.json` & `web3-ethereum-defi-0.9/eth_defi/abi/WETH9Mock.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/Base64Test.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/Base64Test.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/BitMathEchidnaTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/BitMathEchidnaTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/BitMathTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/BitMathTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/ERC721Permit.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/ERC721Permit.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/FullMathEchidnaTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/FullMathEchidnaTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/FullMathTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/FullMathTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IERC1271.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IERC1271.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IERC20Metadata.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IERC20Metadata.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IERC20Minimal.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IERC20Minimal.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IERC20PermitAllowed.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IERC20PermitAllowed.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IERC721Permit.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IERC721Permit.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IMulticall.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IMulticall.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/INonfungiblePositionManager.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/INonfungiblePositionManager.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/INonfungibleTokenPositionDescriptor.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/INonfungibleTokenPositionDescriptor.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IPeripheryImmutableState.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IPeripheryImmutableState.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IPeripheryPayments.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IPeripheryPayments.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IPeripheryPaymentsWithFee.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IPeripheryPaymentsWithFee.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IPoolInitializer.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IPoolInitializer.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IQuoter.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IQuoter.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IQuoterV2.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IQuoterV2.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/ISelfPermit.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/ISelfPermit.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/ISwapRouter.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/ISwapRouter.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/ITickLens.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/ITickLens.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3Factory.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3Factory.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3FlashCallback.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3FlashCallback.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3MintCallback.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3MintCallback.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3Pool.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3Pool.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolActions.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolActions.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolDeployer.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolDeployer.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolDerivedState.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolDerivedState.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolEvents.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolEvents.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolImmutables.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolImmutables.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolOwnerActions.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolOwnerActions.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3PoolState.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3PoolState.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IUniswapV3SwapCallback.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IUniswapV3SwapCallback.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IV3Migrator.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IV3Migrator.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/IWETH9.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/IWETH9.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/LiquidityAmountsTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/LiquidityAmountsTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/LiquidityManagement.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/LiquidityManagement.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/LiquidityMathTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/LiquidityMathTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/LowGasSafeMathEchidnaTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/LowGasSafeMathEchidnaTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/MockObservable.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/MockObservable.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/MockObservations.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/MockObservations.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/MockTimeNonfungiblePositionManager.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/MockTimeNonfungiblePositionManager.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/MockTimeSwapRouter.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/MockTimeSwapRouter.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/MockTimeUniswapV3Pool.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/MockTimeUniswapV3Pool.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/MockTimeUniswapV3PoolDeployer.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/MockTimeUniswapV3PoolDeployer.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/Multicall.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/Multicall.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NFTDescriptor.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NFTDescriptor.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NFTDescriptorTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NFTDescriptorTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NoDelegateCallTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NoDelegateCallTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NonfungiblePositionManager.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NonfungiblePositionManager.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NonfungiblePositionManagerPositionsGasTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NonfungiblePositionManagerPositionsGasTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/NonfungibleTokenPositionDescriptor.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/NonfungibleTokenPositionDescriptor.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/OracleEchidnaTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/OracleEchidnaTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/OracleTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/OracleTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PairFlash.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PairFlash.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PathTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PathTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PeripheryImmutableState.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PeripheryImmutableState.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PeripheryImmutableStateTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PeripheryImmutableStateTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PeripheryPayments.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PeripheryPayments.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PeripheryPaymentsWithFee.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PeripheryPaymentsWithFee.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PoolAddressTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PoolAddressTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PoolInitializer.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PoolInitializer.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PoolTicksCounterTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PoolTicksCounterTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/PositionValueTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/PositionValueTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/Quoter.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/Quoter.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/QuoterV2.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/QuoterV2.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SelfPermit.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SelfPermit.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SelfPermitTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SelfPermitTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SqrtPriceMathEchidnaTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SqrtPriceMathEchidnaTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SqrtPriceMathTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SqrtPriceMathTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SwapMathEchidnaTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SwapMathEchidnaTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SwapMathTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SwapMathTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/SwapRouter.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/SwapRouter.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestCallbackValidation.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestCallbackValidation.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestERC20.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestERC20.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestERC20Metadata.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestERC20Metadata.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestERC20PermitAllowed.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestERC20PermitAllowed.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestMulticall.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestMulticall.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestPositionNFTOwner.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestPositionNFTOwner.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestUniswapV3Callee.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestUniswapV3Callee.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestUniswapV3ReentrantCallee.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestUniswapV3ReentrantCallee.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestUniswapV3Router.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestUniswapV3Router.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TestUniswapV3SwapPay.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TestUniswapV3SwapPay.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickBitmapEchidnaTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickBitmapEchidnaTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickBitmapTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickBitmapTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickEchidnaTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickEchidnaTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickLens.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickLens.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickLensTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickLensTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickMathEchidnaTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickMathEchidnaTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickMathTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickMathTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickOverflowSafetyEchidnaTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickOverflowSafetyEchidnaTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/TickTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/TickTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/UniswapInterfaceMulticall.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/UniswapInterfaceMulticall.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/UniswapV3Factory.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/UniswapV3Factory.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/UniswapV3Pool.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/UniswapV3Pool.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/UniswapV3PoolDeployer.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/UniswapV3PoolDeployer.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/UniswapV3PoolSwapTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/UniswapV3PoolSwapTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/UnsafeMathEchidnaTest.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/UnsafeMathEchidnaTest.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi/uniswap_v3/V3Migrator.json` & `web3-ethereum-defi-0.9/eth_defi/abi/uniswap_v3/V3Migrator.json`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/abi.py` & `web3-ethereum-defi-0.9/eth_defi/abi.py`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/balances.py` & `web3-ethereum-defi-0.9/eth_defi/balances.py`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/deploy.py` & `web3-ethereum-defi-0.9/eth_defi/deploy.py`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/event.py` & `web3-ethereum-defi-0.9/eth_defi/event.py`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/ganache.py` & `web3-ethereum-defi-0.9/eth_defi/ganache.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 .. code-block:: shell
 
     npm install -g ganache
 
 For more information about Ganache see
 
 - `Ganache CLI command line documentation <https://github.com/trufflesuite/ganache#documentation>`_
+
 - `Aave Web.py example <https://github.com/PatrickAlphaC/aave_web3_py>`_
+
 - `QuickNode how to fork mainnet with Ganache tutorial <https://www.quicknode.com/guides/web3-sdks/how-to-fork-ethereum-blockchain-with-ganache>`_
 
 `Most of this code is lifted from Brownie project (MIT) <https://github.com/eth-brownie/brownie/blob/master/brownie/network/rpc/ganache.py>`_
 and it is not properly cleaned up yet.
 
 """
 
@@ -40,14 +42,15 @@
 from hexbytes import HexBytes
 from psutil import NoSuchProcess
 from web3 import HTTPProvider, Web3
 from web3.types import Wei
 
 from eth_defi.utils import is_localhost_port_listening
 
+
 logger = logging.getLogger(__name__)
 
 
 EVM_EQUIVALENTS = {"atlantis": "byzantium", "agharta": "petersburg"}
 
 # https://github.com/trufflesuite/ganache
 CLI_FLAGS = {
@@ -326,29 +329,38 @@
             receipt = web3.eth.get_transaction_receipt(tx_hash)
             assert receipt.status == 1, "BUSD transfer reverted"
 
             assert busd.functions.balanceOf(user_1.address).call() == 500*10**18
 
     `See the full example in tests source code <https://github.com/tradingstrategy-ai/web3-ethereum-defi/blob/master/tests/test_ganache.py>`_.
 
+    Polygon needs to set a specific EVM version:
+
+    .. code-block:: python
+
+            mainnet_rpc = os.environ["POLYGON_JSON_RPC"]
+            launch = fork_network(mainnet_rpc, evm_version="istanbul")
+
     If `ganache-cli` refuses to terminate properly, you can kill a process by a port with:
 
     .. code-block:: shell
 
         # Kill any process listening to localhost:19999
         kill -SIGKILL $(lsof -ti:19999)
 
     This function uses Python logging subsystem. If you want to see error/info/debug logs with `pytest` you can do:
 
     .. code-block:: shell
 
         pytest --log-cli-level=debug
 
     For public JSON-RPC endpoints check
+
     - `BNB chain documentation <https://docs.binance.org/smart-chain/developer/rpc.html>`_
+
     - `ethereumnodes.com <https://ethereumnodes.com/>`_
 
     :param cmd: Override `ganache-cli` command. If not given we look up from `PATH`.
     :param json_rpc_url: HTTP JSON-RPC URL of the network we want to fork
     :param unlocked_addresses: List of addresses of which ownership we take to allow test code to transact as them
     :param port: Localhost port we bind for Ganache JSON-RPC
     :param launch_wait_seconds: How long we wait ganache-cli to start until giving up
```

### Comparing `web3-ethereum-defi-0.8/eth_defi/gas.py` & `web3-ethereum-defi-0.9/eth_defi/gas.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,29 +18,41 @@
 
     #: Post London hard work
     london = "london"
 
 
 @dataclass
 class GasPriceSuggestion:
+    """Gas price details.
 
+    Capture the necessary information for the gas price to used during the transaction building.
+
+    - EIP-1559 London hard fork chains (Ethereumm mainnet)
+
+    - Legacy EVM: Polygon, BNB Chain
+    """
+
+    #: How the gas price was determined
     method: GasPriceMethod
 
     #: Non London hard fork chains
     legacy_gas_price: Optional[int] = None
 
     #: London hard fork chains
     base_fee: Optional[int] = None
 
     #: London hard fork chains
     max_priority_fee_per_gas: Optional[int] = None
 
     #: London hard fork chains
     max_fee_per_gas: Optional[int] = None
 
+    def __repr__(self):
+        return f"<Gas pricing method:{self.method.name} base:{self.base_fee} priority:{self.max_priority_fee_per_gas} max:{self.max_fee_per_gas} legacy:{self.legacy_gas_price}>"
+
 
 def estimate_gas_fees(web3: Web3) -> GasPriceSuggestion:
     """Get a good gas price for a transaction.
 
     TODO: This is non-optimal, first draft implementation.
     """
```

### Comparing `web3-ethereum-defi-0.8/eth_defi/hotwallet.py` & `web3-ethereum-defi-0.9/eth_defi/hotwallet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Utilities for managing hot wallets."""
 
 import logging
 from decimal import Decimal
 from typing import Optional, NamedTuple
 
 from eth_account import Account
-from eth_account.datastructures import SignedTransaction, __getitem__
+from eth_account.datastructures import __getitem__
 from eth_account.signers.local import LocalAccount
 from hexbytes import HexBytes
 from web3 import Web3
 
+from eth_defi.tx import decode_signed_transaction
 
 logger = logging.getLogger(__name__)
 
 
 class SignedTransactionWithNonce(NamedTuple):
     """Helper class to pass around the used nonce when signing txs from the wallet."""
     rawTransaction: HexBytes
@@ -33,14 +34,19 @@
     A hot wallet maintains an unecrypted private key of an Ethereum address in the process memory.
     It is able to sign transactions.
 
     This particular hot wallet implementation carries the information of allocated tx nonces with us.
     This allows us to prepare multiple transactions from the same account upfront.
 
     `See also how to create private keys from command line <https://ethereum.stackexchange.com/q/82926/620>`_.
+
+    .. note ::
+
+        Not thread safe. Manages consumed nonce counter locally.
+
     """
 
     def __init__(self, account: LocalAccount):
         self.account = account
         self.current_nonce: Optional[int] = None
 
     @property
@@ -68,14 +74,15 @@
         """Signs a transaction and allocates a nonce for it.
 
         :param: Ethereum transaction data as a dict. This is modified in-place to include nonce.
         """
         assert "nonce" not in tx
         tx["nonce"] = self.allocate_nonce()
         _signed = self.account.sign_transaction(tx)
+        decode_signed_transaction(_signed.rawTransaction)
         signed = SignedTransactionWithNonce(
             rawTransaction=_signed.rawTransaction,
             hash=_signed.hash,
             v=_signed.v,
             r=_signed.r,
             s=_signed.s,
             nonce=tx["nonce"],
```

### Comparing `web3-ethereum-defi-0.8/eth_defi/revert_reason.py` & `web3-ethereum-defi-0.9/eth_defi/revert_reason.py`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/token.py` & `web3-ethereum-defi-0.9/eth_defi/token.py`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/txmonitor.py` & `web3-ethereum-defi-0.9/eth_defi/confirmation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-"""Transaction broadcasting and monitoring."""
+"""Transaction broadcasting, completion monitoring and confirmations."""
 
 import datetime
 import logging
 import time
-from typing import Dict, List, Set
+from typing import Dict, List, Set, Union
 
 from eth_account.datastructures import SignedTransaction
 from hexbytes import HexBytes
 from web3 import Web3
 from web3.exceptions import TransactionNotFound
 
 from eth_defi.hotwallet import SignedTransactionWithNonce
@@ -17,15 +17,15 @@
 
 class ConfirmationTimedOut(Exception):
     """We exceeded the transaction confirmation timeout."""
 
 
 def wait_transactions_to_complete(
     web3: Web3,
-    txs: List[HexBytes],
+    txs: List[Union[HexBytes, str]],
     confirmation_block_count: int = 0,
     max_timeout=datetime.timedelta(minutes=5),
     poll_delay=datetime.timedelta(seconds=1),
 ) -> Dict[HexBytes, dict]:
     """Watch multiple transactions executed at parallel.
 
     Use simple poll loop to wait all transactions to complete.
@@ -167,15 +167,15 @@
 
                 time.sleep(broadcast_sleep)
                 logger.warning("Rebroadcasting %s, attempts left %d", hash.hex(), attempt)
                 hash = web3.eth.send_raw_transaction(tx.rawTransaction)
                 attempt -= 1
             assert tx_data, f"Could not read broadcasted transaction back from the node {hash.hex()}"
         else:
-            logger.info("We are not going to try to broadcast too hard. work_around_bad_nodes:%s, confirmation_block_count:%d, chain_id:%d", work_around_bad_nodes, confirmation_block_count, chain_id)
+            logger.debug("We are not going to try to broadcast too hard. work_around_bad_nodes:%s, confirmation_block_count:%d, chain_id:%d", work_around_bad_nodes, confirmation_block_count, chain_id)
 
         hashes.append(hash)
 
     return hashes
 
 
 def broadcast_and_wait_transactions_to_complete(
```

### Comparing `web3-ethereum-defi-0.8/eth_defi/uniswap_v2/analysis.py` & `web3-ethereum-defi-0.9/eth_defi/uniswap_v2/analysis.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List, Optional, Union
 
 from eth_defi.revert_reason import fetch_transaction_revert_reason
 from eth_typing import HexAddress
 from web3 import Web3
 from web3.logs import DISCARD
 
-from eth_defi.abi import get_contract, get_transaction_data_field
+from eth_defi.abi import get_transaction_data_field
 from eth_defi.token import fetch_erc20_details
 from eth_defi.uniswap_v2.deployment import UniswapV2Deployment
 
 
 @dataclass
 class TradeResult:
     """A base class for Success/Fail trade result."""
@@ -56,15 +56,15 @@
     The transaction reverted for a reason or another.
     """
 
     #: Revert reason if we managed to extract one
     revert_reason: Optional[str] = None
 
 
-def analyse_trade(web3: Web3, uniswap: UniswapV2Deployment, tx_hash: hash) -> Union[TradeSuccess, TradeFail]:
+def analyse_trade_by_hash(web3: Web3, uniswap: UniswapV2Deployment, tx_hash: str) -> Union[TradeSuccess, TradeFail]:
     """Analyse details of a Uniswap trade based on a transaction id.
 
     Analyses trade fees, etc. based on the event signatures in the transaction.
     Works only simp;e trades.
 
     Currently only supports simple analysis where there is one input token
     and one output token.
@@ -79,25 +79,78 @@
         assert analysis.get_effective_gas_price_gwei() == 1  # What gas was paid for this price
 
     .. note ::
 
         This code is still much under development and unlikely to support any
         advanced use cases yet.
 
-    :param tx_receipt: Transaction receipt for the swap
-    :return: `TradeSuccess` or `TradeFail` analysis
+    :param web3:
+        Web3 instance
+    :param uniswap:
+        Uniswap deployment description
+    :param tx_hash:
+        Transaction hash as a string
+    :return:
+        :py:class:`TradeSuccess` or :py:class:`TradeFail` instance
     """
 
-    pair = get_contract(web3, "UniswapV2Pair.json")
+    pair = uniswap.PairContract
 
     # Example tx https://etherscan.io/tx/0xa8e6d47fb1429c7aec9d30332eafaeb515c8dfa73ab413c48560d8d6060c3193#eventlog
     # swapExactTokensForTokens
 
     tx = web3.eth.get_transaction(tx_hash)
     tx_receipt = web3.eth.get_transaction_receipt(tx_hash)
+    return analyse_trade_by_receipt(web3, uniswap, tx, tx_hash, tx_receipt)
+
+
+def analyse_trade_by_receipt(web3: Web3, uniswap: UniswapV2Deployment, tx: dict, tx_hash: str, tx_receipt: dict) -> Union[TradeSuccess, TradeFail]:
+    """Analyse details of a Uniswap trade based on already received receipt.
+
+    See also :py:func:`analyse_trade_by_hash`.
+    This function is more ideal for the cases where you know your transaction is already confirmed
+    and you do not need to poll the chain for a receipt.
+
+    Example:
+
+    .. code-block:: python
+
+        tx_hash = router.functions.swapExactTokensForTokens(
+            all_weth_amount,
+            0,
+            reverse_path,
+            user_1,
+            FOREVER_DEADLINE,
+        ).transact({"from": user_1})
+
+        tx = web3.eth.get_transaction(tx_hash)
+        receipt = web3.eth.get_transaction_receipt(tx_hash)
+
+        analysis = analyse_trade_by_receipt(web3, uniswap_v2, tx, tx_hash, receipt)
+        assert isinstance(analysis, TradeSuccess)
+        assert analysis.price == pytest.approx(Decimal("1744.899124998896692270848706"))
+
+    :param web3:
+        Web3 instance
+    :param uniswap:
+        Uniswap deployment description
+    :param tx:
+        Transaction data as a dictionary: needs to have `data` or `input` field to decode
+    :param tx_hash:
+        Transaction hash: needed for the call for the revert reason)
+    :param tx_receipt:
+        Transaction receipt to analyse
+    :return:
+        :py:class:`TradeSuccess` or :py:class:`TradeFail` instance
+    """
+
+    pair = uniswap.PairContract
+
+    # Example tx https://etherscan.io/tx/0xa8e6d47fb1429c7aec9d30332eafaeb515c8dfa73ab413c48560d8d6060c3193#eventlog
+    # swapExactTokensForTokens
 
     router = uniswap.router
     assert tx_receipt["to"] == router.address, f"For now, we can only analyze naive trades to the router. This tx was to {tx_receipt['to']}, router is {router.address}"
 
     effective_gas_price = tx_receipt.get("effectiveGasPrice", 0)
     gas_used = tx_receipt["gasUsed"]
 
@@ -159,8 +212,8 @@
 
 _GOOD_TRANSFER_SIGNATURES = (
     # https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/IERC20.sol#L75
     "Transfer(address,address,uint)",
     # WETH9 wtf Transfer()
     # https://github.com/gnosis/canonical-weth/blob/master/contracts/WETH9.sol#L24
     "Transfer(address,address,uint,uint)",
-)
+)
```

### Comparing `web3-ethereum-defi-0.8/eth_defi/uniswap_v2/deployment.py` & `web3-ethereum-defi-0.9/eth_defi/uniswap_v2/deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,26 +11,34 @@
 - QuickSwap
 
 - TraderJoe
 
 Under the hood we are using `SushiSwap v2 contracts <github.com/sushiswap/sushiswap>`_ for the deployment.
 """
 from dataclasses import dataclass
-from typing import Optional, Union
+from typing import Optional, Union, Tuple
 
-from eth_typing import HexAddress, HexStr
+from eth_typing import HexAddress, HexStr, ChecksumAddress
 from web3 import Web3
 from web3.contract import Contract
 
 from eth_defi.abi import get_contract, get_deployed_contract
 from eth_defi.deploy import deploy_contract
 
+
+#: A constant to tell the trade won't expire
+from eth_defi.uniswap_v2.utils import pair_for, sort_tokens
+
 FOREVER_DEADLINE = 2**63
 
 
+#: A constant to tell we do not know or care about pair init code hash for this Uni v2 deploymeny
+INIT_CODE_HASH_MISSING = "0x01"
+
+
 @dataclass(frozen=True)
 class UniswapV2Deployment:
     """Describe Uniswap v2 deployment."""
 
     #: The Web3 instance for which all the contracts here are bound
     web3: Web3
 
@@ -51,14 +59,21 @@
     init_code_hash: HexStr
 
     #: Pair contract proxy class.
     #: Used to manipulate the underlying polls.
     #: See `UniswapV2Pair` smartc contract for details.
     PairContract: Contract
 
+    def pair_for(self, token_a: str, token_b: str) -> Tuple[ChecksumAddress, HexAddress, HexAddress]:
+        """Calculate CREATE2 contract address for a trading pair."""
+        (token0, token1) = sort_tokens(token_a, token_b)
+        return (Web3.toChecksumAddress(pair_for(self.factory.address, token0, token1, self.init_code_hash)),
+                token0,
+                token1)
+
 
 def deploy_factory_sushi(web3: Web3, deployer: str) -> Contract:
     """Deploy a Uniswap V2 factory contract.
 
     This deployment has to be the init code hash hard coded in `UniswapV2Library.sol`.
     We specifically deploy a hash compatible Sushiv2Factory. This makes
     the Uniswap deployment non-recompilable, as the source code files refer to the hashes
@@ -235,21 +250,46 @@
         weth,
         router,
         init_code_hash,
         PairContract,
     )
 
 
+def mock_partial_deployment_for_analysis(web3: Web3, router_address: str) -> UniswapV2Deployment:
+    """Create a Uniswap deployment that is only usable in trade analysis.
+
+    Router and pair is all we need.
+
+    TODO: This function is likely to change / relocate.
+    """
+
+    factory = None
+    init_code_hash = INIT_CODE_HASH_MISSING
+    router = get_deployed_contract(web3, "UniswapV2Router02.json", router_address)
+    PairContract = get_contract(web3, "UniswapV2Pair.json")
+    weth = None
+    return UniswapV2Deployment(
+        web3,
+        factory,
+        weth,
+        router,
+        init_code_hash,
+        PairContract,
+    )
+
+
 # Getting the byte code as https://ethereum.stackexchange.com/questions/77528/web3-eth-getcode-doesnt-return-the-data-shown-on-etherscan
 # Taken from https://etherscan.io/address/0xC0AEe478e3658e2610c5F7A4A2E1777cE9e4f2Ac#code
 _SUSHI_FACTORY_BYTECODE = """0x608060405234801561001057600080fd5b50600436106100a95760003560e01c80637cd07e47116100715780637cd07e47146101395780639aab924814610141578063a2e74af614610149578063c9c653961461016f578063e6a439051461019d578063f46901ed146101cb576100a9565b8063017e7e58146100ae578063094b7415146100d25780631e3dd18b146100da57806323cf3118146100f7578063574f2ba31461011f575b600080fd5b6100b66101f1565b604080516001600160a01b039092168252519081900360200190f35b6100b6610200565b6100b6600480360360208110156100f057600080fd5b503561020f565b61011d6004803603602081101561010d57600080fd5b50356001600160a01b0316610236565b005b6101276102ae565b60408051918252519081900360200190f35b6100b66102b4565b6101276102c3565b61011d6004803603602081101561015f57600080fd5b50356001600160a01b03166102f5565b6100b66004803603604081101561018557600080fd5b506001600160a01b038135811691602001351661036d565b6100b6600480360360408110156101b357600080fd5b506001600160a01b0381358116916020013516610698565b61011d600480360360208110156101e157600080fd5b50356001600160a01b03166106be565b6000546001600160a01b031681565b6001546001600160a01b031681565b6004818154811061021c57fe5b6000918252602090912001546001600160a01b0316905081565b6001546001600160a01b0316331461028c576040805162461bcd60e51b81526020600482015260146024820152732ab734b9bbb0b82b191d102327a92124a22222a760611b604482015290519081900360640190fd5b600280546001600160a01b0319166001600160a01b0392909216919091179055565b60045490565b6002546001600160a01b031681565b6000604051806020016102d590610736565b6020820181038252601f19601f8201166040525080519060200120905090565b6001546001600160a01b0316331461034b576040805162461bcd60e51b81526020600482015260146024820152732ab734b9bbb0b82b191d102327a92124a22222a760611b604482015290519081900360640190fd5b600180546001600160a01b0319166001600160a01b0392909216919091179055565b6000816001600160a01b0316836001600160a01b031614156103d6576040805162461bcd60e51b815260206004820152601e60248201527f556e697377617056323a204944454e544943414c5f4144445245535345530000604482015290519081900360640190fd5b600080836001600160a01b0316856001600160a01b0316106103f95783856103fc565b84845b90925090506001600160a01b03821661045c576040805162461bcd60e51b815260206004820152601760248201527f556e697377617056323a205a45524f5f41444452455353000000000000000000604482015290519081900360640190fd5b6001600160a01b038281166000908152600360209081526040808320858516845290915290205416156104cf576040805162461bcd60e51b8152602060048201526016602482015275556e697377617056323a20504149525f45584953545360501b604482015290519081900360640190fd5b6060604051806020016104e190610736565b6020820181038252601f19601f8201166040525090506000838360405160200180836001600160a01b031660601b8152601401826001600160a01b031660601b815260140192505050604051602081830303815290604052805190602001209050808251602084016000f59450846001600160a01b031663485cc95585856040518363ffffffff1660e01b815260040180836001600160a01b03168152602001826001600160a01b0316815260200192505050600060405180830381600087803b1580156105ae57600080fd5b505af11580156105c2573d6000803e3d6000fd5b505050506001600160a01b0384811660008181526003602081815260408084208987168086529083528185208054978d166001600160a01b031998891681179091559383528185208686528352818520805488168517905560048054600181018255958190527f8a35acfbc15ff81a39ae7d344fd709f28e8600b4aa8c65c6b64bfe7fe36bd19b90950180549097168417909655925483519283529082015281517f0d3648bd0f6ba80134a33ba9275ac585d9d315f0ad8355cddefde31afa28d0e9929181900390910190a35050505092915050565b60036020908152600092835260408084209091529082529020546001600160a01b031681565b6001546001600160a01b03163314610714576040805162461bcd60e51b81526020600482015260146024820152732ab734b9bbb0b82b191d102327a92124a22222a760611b604482015290519081900360640190fd5b600080546001600160a01b0319166001600160a01b0392909216919091179055565b612487806107448339019056fe60806040526001600c5534801561001557600080fd5b50604080518082018252601281527129bab9b434a9bbb0b8102628102a37b5b2b760711b6020918201528151808301835260018152603160f81b9082015281517f8b73c3c69bb8fe3d512ecc4cf759cc79239f7b179b0ffacaa9a75d522b39400f818301527fefbffe65652a145845c9bc8d0532945be6b9830fe1e9966c887bd298e551ac83818401527fc89efdaa54c0f20c7adf612882df0950f5a951637e0307cdcb4c672f298b8bc660608201524660808201523060a0808301919091528351808303909101815260c09091019092528151910120600355600580546001600160a01b03191633179055612377806101106000396000f3fe608060405234801561001057600080fd5b50600436106101a95760003560e01c80636a627842116100f9578063ba9a7a5611610097578063d21220a711610071578063d21220a714610534578063d505accf1461053c578063dd62ed3e1461058d578063fff6cae9146105bb576101a9565b8063ba9a7a56146104fe578063bc25cf7714610506578063c45a01551461052c576101a9565b80637ecebe00116100d35780637ecebe001461046557806389afcb441461048b57806395d89b41146104ca578063a9059cbb146104d2576101a9565b80636a6278421461041157806370a08231146104375780637464fc3d1461045d576101a9565b806323b872dd116101665780633644e515116101405780633644e515146103cb578063485cc955146103d35780635909c0d5146104015780635a3d549314610409576101a9565b806323b872dd1461036f57806330adf81f146103a5578063313ce567146103ad576101a9565b8063022c0d9f146101ae57806306fdde031461023c5780630902f1ac146102b9578063095ea7b3146102f15780630dfe16811461033157806318160ddd14610355575b600080fd5b61023a600480360360808110156101c457600080fd5b8135916020810135916001600160a01b0360408301351691908101906080810160608201356401000000008111156101fb57600080fd5b82018360208201111561020d57600080fd5b8035906020019184600183028401116401000000008311171561022f57600080fd5b5090925090506105c3565b005b610244610acb565b6040805160208082528351818301528351919283929083019185019080838360005b8381101561027e578181015183820152602001610266565b50505050905090810190601f1680156102ab5780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b6102c1610af9565b604080516001600160701b03948516815292909316602083015263ffffffff168183015290519081900360600190f35b61031d6004803603604081101561030757600080fd5b506001600160a01b038135169060200135610b23565b604080519115158252519081900360200190f35b610339610b3a565b604080516001600160a01b039092168252519081900360200190f35b61035d610b49565b60408051918252519081900360200190f35b61031d6004803603606081101561038557600080fd5b506001600160a01b03813581169160208101359091169060400135610b4f565b61035d610be3565b6103b5610c07565b6040805160ff9092168252519081900360200190f35b61035d610c0c565b61023a600480360360408110156103e957600080fd5b506001600160a01b0381358116916020013516610c12565b61035d610c96565b61035d610c9c565b61035d6004803603602081101561042757600080fd5b50356001600160a01b0316610ca2565b61035d6004803603602081101561044d57600080fd5b50356001600160a01b031661111e565b61035d611130565b61035d6004803603602081101561047b57600080fd5b50356001600160a01b0316611136565b6104b1600480360360208110156104a157600080fd5b50356001600160a01b0316611148565b6040805192835260208301919091528051918290030190f35b6102446114dc565b61031d600480360360408110156104e857600080fd5b506001600160a01b0381351690602001356114fb565b61035d611508565b61023a6004803603602081101561051c57600080fd5b50356001600160a01b031661150e565b610339611680565b61033961168f565b61023a600480360360e081101561055257600080fd5b506001600160a01b03813581169160208101359091169060408101359060608101359060ff6080820135169060a08101359060c0013561169e565b61035d600480360360408110156105a357600080fd5b506001600160a01b03813581169160200135166118a0565b61023a6118bd565b600c5460011461060e576040805162461bcd60e51b8152602060048201526011602482015270155b9a5cddd85c158c8e881313d0d2d151607a1b604482015290519081900360640190fd5b6000600c55841515806106215750600084115b61065c5760405162461bcd60e51b81526004018080602001828103825260258152602001806122886025913960400191505060405180910390fd5b600080610667610af9565b5091509150816001600160701b03168710801561068c5750806001600160701b031686105b6106c75760405162461bcd60e51b81526004018080602001828103825260218152602001806122d16021913960400191505060405180910390fd5b60065460075460009182916001600160a01b039182169190811690891682148015906107055750806001600160a01b0316896001600160a01b031614155b61074e576040805162461bcd60e51b8152602060048201526015602482015274556e697377617056323a20494e56414c49445f544f60581b604482015290519081900360640190fd5b8a1561075f5761075f828a8d611a1f565b891561077057610770818a8c611a1f565b861561082257886001600160a01b03166310d1e85c338d8d8c8c6040518663ffffffff1660e01b815260040180866001600160a01b03168152602001858152602001848152602001806020018281038252848482818152602001925080828437600081840152601f19601f8201169050808301925050509650505050505050600060405180830381600087803b15801561080957600080fd5b505af115801561081d573d6000803e3d6000fd5b505050505b604080516370a0823160e01b815230600482015290516001600160a01b038416916370a08231916024808301926020929190829003018186803b15801561086857600080fd5b505afa15801561087c573d6000803e3d6000fd5b505050506040513d602081101561089257600080fd5b5051604080516370a0823160e01b815230600482015290519195506001600160a01b038316916370a0823191602480820192602092909190829003018186803b1580156108de57600080fd5b505afa1580156108f2573d6000803e3d6000fd5b505050506040513d602081101561090857600080fd5b5051925060009150506001600160701b0385168a9003831161092b57600061093a565b89856001600160701b03160383035b9050600089856001600160701b0316038311610957576000610966565b89856001600160701b03160383035b905060008211806109775750600081115b6109b25760405162461bcd60e51b81526004018080602001828103825260248152602001806122ad6024913960400191505060405180910390fd5b60006109d46109c2846003611bb9565b6109ce876103e8611bb9565b90611c1c565b905060006109e66109c2846003611bb9565b9050610a0b620f4240610a056001600160701b038b8116908b16611bb9565b90611bb9565b610a158383611bb9565b1015610a57576040805162461bcd60e51b815260206004820152600c60248201526b556e697377617056323a204b60a01b604482015290519081900360640190fd5b5050610a6584848888611c6c565b60408051838152602081018390528082018d9052606081018c905290516001600160a01b038b169133917fd78ad95fa46c994b6551d0da85fc275fe613ce37657fb8d5e3d130840159d8229181900360800190a350506001600c55505050505050505050565b6040518060400160405280601281526020017129bab9b434a9bbb0b8102628102a37b5b2b760711b81525081565b6008546001600160701b0380821692600160701b830490911691600160e01b900463ffffffff1690565b6000610b30338484611e2b565b5060015b92915050565b6006546001600160a01b031681565b60005481565b6001600160a01b038316600090815260026020908152604080832033845290915281205460001914610bce576001600160a01b0384166000908152600260209081526040808320338452909152902054610ba99083611c1c565b6001600160a01b03851660009081526002602090815260408083203384529091529020555b610bd9848484611e8d565b5060019392505050565b7f6e71edae12b1b97f4d1f60370fef10105fa2faae0126114a169c64845d6126c981565b601281565b60035481565b6005546001600160a01b03163314610c68576040805162461bcd60e51b81526020600482015260146024820152732ab734b9bbb0b82b191d102327a92124a22222a760611b604482015290519081900360640190fd5b600680546001600160a01b039384166001600160a01b03199182161790915560078054929093169116179055565b60095481565b600a5481565b6000600c54600114610cef576040805162461bcd60e51b8152602060048201526011602482015270155b9a5cddd85c158c8e881313d0d2d151607a1b604482015290519081900360640190fd5b6000600c81905580610cff610af9565b50600654604080516370a0823160e01b815230600482015290519395509193506000926001600160a01b03909116916370a08231916024808301926020929190829003018186803b158015610d5357600080fd5b505afa158015610d67573d6000803e3d6000fd5b505050506040513d6020811015610d7d57600080fd5b5051600754604080516370a0823160e01b815230600482015290519293506000926001600160a01b03909216916370a0823191602480820192602092909190829003018186803b158015610dd057600080fd5b505afa158015610de4573d6000803e3d6000fd5b505050506040513d6020811015610dfa57600080fd5b505190506000610e13836001600160701b038716611c1c565b90506000610e2a836001600160701b038716611c1c565b90506000610e388787611f3b565b6000549091508061100f5760055460408051637cd07e4760e01b815290516000926001600160a01b031691637cd07e47916004808301926020929190829003018186803b158015610e8857600080fd5b505afa158015610e9c573d6000803e3d6000fd5b505050506040513d6020811015610eb257600080fd5b50519050336001600160a01b0382161415610f8d57806001600160a01b03166340dc0e376040518163ffffffff1660e01b815260040160206040518083038186803b158015610f0057600080fd5b505afa158015610f14573d6000803e3d6000fd5b505050506040513d6020811015610f2a57600080fd5b505199508915801590610f3f57506000198a14155b610f88576040805162461bcd60e51b81526020600482015260156024820152744261642064657369726564206c697175696469747960581b604482015290519081900360640190fd5b611009565b6001600160a01b03811615610fe2576040805162461bcd60e51b815260206004820152601660248201527526bab9ba103737ba103430bb329036b4b3b930ba37b960511b604482015290519081900360640190fd5b610ffa6103e86109ce610ff58888611bb9565b61207b565b995061100960006103e86120cd565b50611052565b61104f6001600160701b0389166110268684611bb9565b8161102d57fe5b046001600160701b0389166110428685611bb9565b8161104957fe5b04612157565b98505b600089116110915760405162461bcd60e51b815260040180806020018281038252602881526020018061231a6028913960400191505060405180910390fd5b61109b8a8a6120cd565b6110a786868a8a611c6c565b81156110d1576008546110cd906001600160701b0380821691600160701b900416611bb9565b600b555b6040805185815260208101859052815133927f4c209b5fc8ad50758f13e2e1088ba56a560dff690a1c6fef26394f4c03821c4f928290030190a250506001600c5550949695505050505050565b60016020526000908152604090205481565b600b5481565b60046020526000908152604090205481565b600080600c54600114611196576040805162461bcd60e51b8152602060048201526011602482015270155b9a5cddd85c158c8e881313d0d2d151607a1b604482015290519081900360640190fd5b6000600c819055806111a6610af9565b50600654600754604080516370a0823160e01b815230600482015290519496509294506001600160a01b039182169391169160009184916370a08231916024808301926020929190829003018186803b15801561120257600080fd5b505afa158015611216573d6000803e3d6000fd5b505050506040513d602081101561122c57600080fd5b5051604080516370a0823160e01b815230600482015290519192506000916001600160a01b038516916370a08231916024808301926020929190829003018186803b15801561127a57600080fd5b505afa15801561128e573d6000803e3d6000fd5b505050506040513d60208110156112a457600080fd5b5051306000908152600160205260408120549192506112c38888611f3b565b600054909150806112d48487611bb9565b816112db57fe5b049a50806112e98486611bb9565b816112f057fe5b04995060008b118015611303575060008a115b61133e5760405162461bcd60e51b81526004018080602001828103825260288152602001806122f26028913960400191505060405180910390fd5b611348308461216f565b611353878d8d611a1f565b61135e868d8c611a1f565b604080516370a0823160e01b815230600482015290516001600160a01b038916916370a08231916024808301926020929190829003018186803b1580156113a457600080fd5b505afa1580156113b8573d6000803e3d6000fd5b505050506040513d60208110156113ce57600080fd5b5051604080516370a0823160e01b815230600482015290519196506001600160a01b038816916370a0823191602480820192602092909190829003018186803b15801561141a57600080fd5b505afa15801561142e573d6000803e3d6000fd5b505050506040513d602081101561144457600080fd5b5051935061145485858b8b611c6c565b811561147e5760085461147a906001600160701b0380821691600160701b900416611bb9565b600b555b604080518c8152602081018c905281516001600160a01b038f169233927fdccd412f0b1252819cb1fd330b93224ca42612892bb3f4f789976e6d81936496929081900390910190a35050505050505050506001600c81905550915091565b604051806040016040528060038152602001620534c560ec1b81525081565b6000610b30338484611e8d565b6103e881565b600c54600114611559576040805162461bcd60e51b8152602060048201526011602482015270155b9a5cddd85c158c8e881313d0d2d151607a1b604482015290519081900360640190fd5b6000600c55600654600754600854604080516370a0823160e01b815230600482015290516001600160a01b03948516949093169261160292859287926115fd926001600160701b03169185916370a0823191602480820192602092909190829003018186803b1580156115cb57600080fd5b505afa1580156115df573d6000803e3d6000fd5b505050506040513d60208110156115f557600080fd5b505190611c1c565b611a1f565b61167681846115fd6008600e9054906101000a90046001600160701b03166001600160701b0316856001600160a01b03166370a08231306040518263ffffffff1660e01b815260040180826001600160a01b0316815260200191505060206040518083038186803b1580156115cb57600080fd5b50506001600c5550565b6005546001600160a01b031681565b6007546001600160a01b031681565b428410156116e8576040805162461bcd60e51b8152602060048201526012602482015271155b9a5cddd85c158c8e881156141254915160721b604482015290519081900360640190fd5b6003546001600160a01b0380891660008181526004602090815260408083208054600180820190925582517f6e71edae12b1b97f4d1f60370fef10105fa2faae0126114a169c64845d6126c98186015280840196909652958d166060860152608085018c905260a085019590955260c08085018b90528151808603909101815260e08501825280519083012061190160f01b6101008601526101028501969096526101228085019690965280518085039096018652610142840180825286519683019690962095839052610162840180825286905260ff89166101828501526101a284018890526101c28401879052519193926101e280820193601f1981019281900390910190855afa158015611803573d6000803e3d6000fd5b5050604051601f1901519150506001600160a01b038116158015906118395750886001600160a01b0316816001600160a01b0316145b61188a576040805162461bcd60e51b815260206004820152601c60248201527f556e697377617056323a20494e56414c49445f5349474e415455524500000000604482015290519081900360640190fd5b611895898989611e2b565b505050505050505050565b600260209081526000928352604080842090915290825290205481565b600c54600114611908576040805162461bcd60e51b8152602060048201526011602482015270155b9a5cddd85c158c8e881313d0d2d151607a1b604482015290519081900360640190fd5b6000600c55600654604080516370a0823160e01b81523060048201529051611a18926001600160a01b0316916370a08231916024808301926020929190829003018186803b15801561195957600080fd5b505afa15801561196d573d6000803e3d6000fd5b505050506040513d602081101561198357600080fd5b5051600754604080516370a0823160e01b815230600482015290516001600160a01b03909216916370a0823191602480820192602092909190829003018186803b1580156119d057600080fd5b505afa1580156119e4573d6000803e3d6000fd5b505050506040513d60208110156119fa57600080fd5b50516008546001600160701b0380821691600160701b900416611c6c565b6001600c55565b604080518082018252601981527f7472616e7366657228616464726573732c75696e74323536290000000000000060209182015281516001600160a01b0385811660248301526044808301869052845180840390910181526064909201845291810180516001600160e01b031663a9059cbb60e01b1781529251815160009460609489169392918291908083835b60208310611acc5780518252601f199092019160209182019101611aad565b6001836020036101000a0380198251168184511680821785525050505050509050019150506000604051808303816000865af19150503d8060008114611b2e576040519150601f19603f3d011682016040523d82523d6000602084013e611b33565b606091505b5091509150818015611b61575080511580611b615750808060200190516020811015611b5e57600080fd5b50515b611bb2576040805162461bcd60e51b815260206004820152601a60248201527f556e697377617056323a205452414e534645525f4641494c4544000000000000604482015290519081900360640190fd5b5050505050565b6000811580611bd457505080820282828281611bd157fe5b04145b610b34576040805162461bcd60e51b815260206004820152601460248201527364732d6d6174682d6d756c2d6f766572666c6f7760601b604482015290519081900360640190fd5b80820382811115610b34576040805162461bcd60e51b815260206004820152601560248201527464732d6d6174682d7375622d756e646572666c6f7760581b604482015290519081900360640190fd5b6001600160701b038411801590611c8a57506001600160701b038311155b611cd1576040805162461bcd60e51b8152602060048201526013602482015272556e697377617056323a204f564552464c4f5760681b604482015290519081900360640190fd5b60085463ffffffff42811691600160e01b90048116820390811615801590611d0157506001600160701b03841615155b8015611d1557506001600160701b03831615155b15611d80578063ffffffff16611d3d85611d2e86612201565b6001600160e01b031690612213565b600980546001600160e01b03929092169290920201905563ffffffff8116611d6884611d2e87612201565b600a80546001600160e01b0392909216929092020190555b600880546dffffffffffffffffffffffffffff19166001600160701b03888116919091176dffffffffffffffffffffffffffff60701b1916600160701b8883168102919091176001600160e01b0316600160e01b63ffffffff871602179283905560408051848416815291909304909116602082015281517f1c411e9a96e071241c2f21f7726b17ae89e3cab4c78be50e062b03a9fffbbad1929181900390910190a1505050505050565b6001600160a01b03808416600081815260026020908152604080832094871680845294825291829020859055815185815291517f8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b9259281900390910190a3505050565b6001600160a01b038316600090815260016020526040902054611eb09082611c1c565b6001600160a01b038085166000908152600160205260408082209390935590841681522054611edf9082612238565b6001600160a01b0380841660008181526001602090815260409182902094909455805185815290519193928716927fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef92918290030190a3505050565b600080600560009054906101000a90046001600160a01b03166001600160a01b031663017e7e586040518163ffffffff1660e01b815260040160206040518083038186803b158015611f8c57600080fd5b505afa158015611fa0573d6000803e3d6000fd5b505050506040513d6020811015611fb657600080fd5b5051600b546001600160a01b038216158015945091925090612067578015612062576000611ff3610ff56001600160701b03888116908816611bb9565b905060006120008361207b565b90508082111561205f5760006120226120198484611c1c565b60005490611bb9565b9050600061203b83612035866005611bb9565b90612238565b9050600081838161204857fe5b049050801561205b5761205b87826120cd565b5050505b50505b612073565b8015612073576000600b555b505092915050565b600060038211156120be575080600160028204015b818110156120b8578091506002818285816120a757fe5b0401816120b057fe5b049050612090565b506120c8565b81156120c8575060015b919050565b6000546120da9082612238565b60009081556001600160a01b0383168152600160205260409020546120ff9082612238565b6001600160a01b03831660008181526001602090815260408083209490945583518581529351929391927fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef9281900390910190a35050565b60008183106121665781612168565b825b9392505050565b6001600160a01b0382166000908152600160205260409020546121929082611c1c565b6001600160a01b038316600090815260016020526040812091909155546121b99082611c1c565b60009081556040805183815290516001600160a01b038516917fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef919081900360200190a35050565b6001600160701b0316600160701b0290565b60006001600160701b0382166001600160e01b0384168161223057fe5b049392505050565b80820182811015610b34576040805162461bcd60e51b815260206004820152601460248201527364732d6d6174682d6164642d6f766572666c6f7760601b604482015290519081900360640190fdfe556e697377617056323a20494e53554646494349454e545f4f55545055545f414d4f554e54556e697377617056323a20494e53554646494349454e545f494e5055545f414d4f554e54556e697377617056323a20494e53554646494349454e545f4c4951554944495459556e697377617056323a20494e53554646494349454e545f4c49515549444954595f4255524e4544556e697377617056323a20494e53554646494349454e545f4c49515549444954595f4d494e544544a2646970667358221220713a8bf21df06433f34b5c9abf186abb737e72524583bdf420105a289791e24864736f6c634300060c0033a26469706673582212209c1e46967e61d91a65487ad45d080a227969fffa0564957df8e023b202f4d62a64736f6c634300060c0033"""
 
+
 # See https://etherscan.io/tx/0x7714c68f1561629b3656da2e4aea1a5b9f1402568398a4396f9d256900230220
 _SUSHI_FACTORY_DEPLOYMENT_DATA = """0x608060405234801561001057600080fd5b50604051612c63380380612c638339818101604052602081101561003357600080fd5b5051600180546001600160a01b0319166001600160a01b03909216919091179055612c00806100636000396000f3fe608060405234801561001057600080fd5b50600436106100a95760003560e01c80637cd07e47116100715780637cd07e47146101395780639aab924814610141578063a2e74af614610149578063c9c653961461016f578063e6a439051461019d578063f46901ed146101cb576100a9565b8063017e7e58146100ae578063094b7415146100d25780631e3dd18b146100da57806323cf3118146100f7578063574f2ba31461011f575b600080fd5b6100b66101f1565b604080516001600160a01b039092168252519081900360200190f35b6100b6610200565b6100b6600480360360208110156100f057600080fd5b503561020f565b61011d6004803603602081101561010d57600080fd5b50356001600160a01b0316610236565b005b6101276102ae565b60408051918252519081900360200190f35b6100b66102b4565b6101276102c3565b61011d6004803603602081101561015f57600080fd5b50356001600160a01b03166102f5565b6100b66004803603604081101561018557600080fd5b506001600160a01b038135811691602001351661036d565b6100b6600480360360408110156101b357600080fd5b506001600160a01b0381358116916020013516610698565b61011d600480360360208110156101e157600080fd5b50356001600160a01b03166106be565b6000546001600160a01b031681565b6001546001600160a01b031681565b6004818154811061021c57fe5b6000918252602090912001546001600160a01b0316905081565b6001546001600160a01b0316331461028c576040805162461bcd60e51b81526020600482015260146024820152732ab734b9bbb0b82b191d102327a92124a22222a760611b604482015290519081900360640190fd5b600280546001600160a01b0319166001600160a01b0392909216919091179055565b60045490565b6002546001600160a01b031681565b6000604051806020016102d590610736565b6020820181038252601f19601f8201166040525080519060200120905090565b6001546001600160a01b0316331461034b576040805162461bcd60e51b81526020600482015260146024820152732ab734b9bbb0b82b191d102327a92124a22222a760611b604482015290519081900360640190fd5b600180546001600160a01b0319166001600160a01b0392909216919091179055565b6000816001600160a01b0316836001600160a01b031614156103d6576040805162461bcd60e51b815260206004820152601e60248201527f556e697377617056323a204944454e544943414c5f4144445245535345530000604482015290519081900360640190fd5b600080836001600160a01b0316856001600160a01b0316106103f95783856103fc565b84845b90925090506001600160a01b03821661045c576040805162461bcd60e51b815260206004820152601760248201527f556e697377617056323a205a45524f5f41444452455353000000000000000000604482015290519081900360640190fd5b6001600160a01b038281166000908152600360209081526040808320858516845290915290205416156104cf576040805162461bcd60e51b8152602060048201526016602482015275556e697377617056323a20504149525f45584953545360501b604482015290519081900360640190fd5b6060604051806020016104e190610736565b6020820181038252601f19601f8201166040525090506000838360405160200180836001600160a01b031660601b8152601401826001600160a01b031660601b815260140192505050604051602081830303815290604052805190602001209050808251602084016000f59450846001600160a01b031663485cc95585856040518363ffffffff1660e01b815260040180836001600160a01b03168152602001826001600160a01b0316815260200192505050600060405180830381600087803b1580156105ae57600080fd5b505af11580156105c2573d6000803e3d6000fd5b505050506001600160a01b0384811660008181526003602081815260408084208987168086529083528185208054978d166001600160a01b031998891681179091559383528185208686528352818520805488168517905560048054600181018255958190527f8a35acfbc15ff81a39ae7d344fd709f28e8600b4aa8c65c6b64bfe7fe36bd19b90950180549097168417909655925483519283529082015281517f0d3648bd0f6ba80134a33ba9275ac585d9d315f0ad8355cddefde31afa28d0e9929181900390910190a35050505092915050565b60036020908152600092835260408084209091529082529020546001600160a01b031681565b6001546001600160a01b03163314610714576040805162461bcd60e51b81526020600482015260146024820152732ab734b9bbb0b82b191d102327a92124a22222a760611b604482015290519081900360640190fd5b600080546001600160a01b0319166001600160a01b0392909216919091179055565b612487806107448339019056fe60806040526001600c5534801561001557600080fd5b50604080518082018252601281527129bab9b434a9bbb0b8102628102a37b5b2b760711b6020918201528151808301835260018152603160f81b9082015281517f8b73c3c69bb8fe3d512ecc4cf759cc79239f7b179b0ffacaa9a75d522b39400f818301527fefbffe65652a145845c9bc8d0532945be6b9830fe1e9966c887bd298e551ac83818401527fc89efdaa54c0f20c7adf612882df0950f5a951637e0307cdcb4c672f298b8bc660608201524660808201523060a0808301919091528351808303909101815260c09091019092528151910120600355600580546001600160a01b03191633179055612377806101106000396000f3fe608060405234801561001057600080fd5b50600436106101a95760003560e01c80636a627842116100f9578063ba9a7a5611610097578063d21220a711610071578063d21220a714610534578063d505accf1461053c578063dd62ed3e1461058d578063fff6cae9146105bb576101a9565b8063ba9a7a56146104fe578063bc25cf7714610506578063c45a01551461052c576101a9565b80637ecebe00116100d35780637ecebe001461046557806389afcb441461048b57806395d89b41146104ca578063a9059cbb146104d2576101a9565b80636a6278421461041157806370a08231146104375780637464fc3d1461045d576101a9565b806323b872dd116101665780633644e515116101405780633644e515146103cb578063485cc955146103d35780635909c0d5146104015780635a3d549314610409576101a9565b806323b872dd1461036f57806330adf81f146103a5578063313ce567146103ad576101a9565b8063022c0d9f146101ae57806306fdde031461023c5780630902f1ac146102b9578063095ea7b3146102f15780630dfe16811461033157806318160ddd14610355575b600080fd5b61023a600480360360808110156101c457600080fd5b8135916020810135916001600160a01b0360408301351691908101906080810160608201356401000000008111156101fb57600080fd5b82018360208201111561020d57600080fd5b8035906020019184600183028401116401000000008311171561022f57600080fd5b5090925090506105c3565b005b610244610acb565b6040805160208082528351818301528351919283929083019185019080838360005b8381101561027e578181015183820152602001610266565b50505050905090810190601f1680156102ab5780820380516001836020036101000a031916815260200191505b509250505060405180910390f35b6102c1610af9565b604080516001600160701b03948516815292909316602083015263ffffffff168183015290519081900360600190f35b61031d6004803603604081101561030757600080fd5b506001600160a01b038135169060200135610b23565b604080519115158252519081900360200190f35b610339610b3a565b604080516001600160a01b039092168252519081900360200190f35b61035d610b49565b60408051918252519081900360200190f35b61031d6004803603606081101561038557600080fd5b506001600160a01b03813581169160208101359091169060400135610b4f565b61035d610be3565b6103b5610c07565b6040805160ff9092168252519081900360200190f35b61035d610c0c565b61023a600480360360408110156103e957600080fd5b506001600160a01b0381358116916020013516610c12565b61035d610c96565b61035d610c9c565b61035d6004803603602081101561042757600080fd5b50356001600160a01b0316610ca2565b61035d6004803603602081101561044d57600080fd5b50356001600160a01b031661111e565b61035d611130565b61035d6004803603602081101561047b57600080fd5b50356001600160a01b0316611136565b6104b1600480360360208110156104a157600080fd5b50356001600160a01b0316611148565b6040805192835260208301919091528051918290030190f35b6102446114dc565b61031d600480360360408110156104e857600080fd5b506001600160a01b0381351690602001356114fb565b61035d611508565b61023a6004803603602081101561051c57600080fd5b50356001600160a01b031661150e565b610339611680565b61033961168f565b61023a600480360360e081101561055257600080fd5b506001600160a01b03813581169160208101359091169060408101359060608101359060ff6080820135169060a08101359060c0013561169e565b61035d600480360360408110156105a357600080fd5b506001600160a01b03813581169160200135166118a0565b61023a6118bd565b600c5460011461060e576040805162461bcd60e51b8152602060048201526011602482015270155b9a5cddd85c158c8e881313d0d2d151607a1b604482015290519081900360640190fd5b6000600c55841515806106215750600084115b61065c5760405162461bcd60e51b81526004018080602001828103825260258152602001806122886025913960400191505060405180910390fd5b600080610667610af9565b5091509150816001600160701b03168710801561068c5750806001600160701b031686105b6106c75760405162461bcd60e51b81526004018080602001828103825260218152602001806122d16021913960400191505060405180910390fd5b60065460075460009182916001600160a01b039182169190811690891682148015906107055750806001600160a01b0316896001600160a01b031614155b61074e576040805162461bcd60e51b8152602060048201526015602482015274556e697377617056323a20494e56414c49445f544f60581b604482015290519081900360640190fd5b8a1561075f5761075f828a8d611a1f565b891561077057610770818a8c611a1f565b861561082257886001600160a01b03166310d1e85c338d8d8c8c6040518663ffffffff1660e01b815260040180866001600160a01b03168152602001858152602001848152602001806020018281038252848482818152602001925080828437600081840152601f19601f8201169050808301925050509650505050505050600060405180830381600087803b15801561080957600080fd5b505af115801561081d573d6000803e3d6000fd5b505050505b604080516370a0823160e01b815230600482015290516001600160a01b038416916370a08231916024808301926020929190829003018186803b15801561086857600080fd5b505afa15801561087c573d6000803e3d6000fd5b505050506040513d602081101561089257600080fd5b5051604080516370a0823160e01b815230600482015290519195506001600160a01b038316916370a0823191602480820192602092909190829003018186803b1580156108de57600080fd5b505afa1580156108f2573d6000803e3d6000fd5b505050506040513d602081101561090857600080fd5b5051925060009150506001600160701b0385168a9003831161092b57600061093a565b89856001600160701b03160383035b9050600089856001600160701b0316038311610957576000610966565b89856001600160701b03160383035b905060008211806109775750600081115b6109b25760405162461bcd60e51b81526004018080602001828103825260248152602001806122ad6024913960400191505060405180910390fd5b60006109d46109c2846003611bb9565b6109ce876103e8611bb9565b90611c1c565b905060006109e66109c2846003611bb9565b9050610a0b620f4240610a056001600160701b038b8116908b16611bb9565b90611bb9565b610a158383611bb9565b1015610a57576040805162461bcd60e51b815260206004820152600c60248201526b556e697377617056323a204b60a01b604482015290519081900360640190fd5b5050610a6584848888611c6c565b60408051838152602081018390528082018d9052606081018c905290516001600160a01b038b169133917fd78ad95fa46c994b6551d0da85fc275fe613ce37657fb8d5e3d130840159d8229181900360800190a350506001600c55505050505050505050565b6040518060400160405280601281526020017129bab9b434a9bbb0b8102628102a37b5b2b760711b81525081565b6008546001600160701b0380821692600160701b830490911691600160e01b900463ffffffff1690565b6000610b30338484611e2b565b5060015b92915050565b6006546001600160a01b031681565b60005481565b6001600160a01b038316600090815260026020908152604080832033845290915281205460001914610bce576001600160a01b0384166000908152600260209081526040808320338452909152902054610ba99083611c1c565b6001600160a01b03851660009081526002602090815260408083203384529091529020555b610bd9848484611e8d565b5060019392505050565b7f6e71edae12b1b97f4d1f60370fef10105fa2faae0126114a169c64845d6126c981565b601281565b60035481565b6005546001600160a01b03163314610c68576040805162461bcd60e51b81526020600482015260146024820152732ab734b9bbb0b82b191d102327a92124a22222a760611b604482015290519081900360640190fd5b600680546001600160a01b039384166001600160a01b03199182161790915560078054929093169116179055565b60095481565b600a5481565b6000600c54600114610cef576040805162461bcd60e51b8152602060048201526011602482015270155b9a5cddd85c158c8e881313d0d2d151607a1b604482015290519081900360640190fd5b6000600c81905580610cff610af9565b50600654604080516370a0823160e01b815230600482015290519395509193506000926001600160a01b03909116916370a08231916024808301926020929190829003018186803b158015610d5357600080fd5b505afa158015610d67573d6000803e3d6000fd5b505050506040513d6020811015610d7d57600080fd5b5051600754604080516370a0823160e01b815230600482015290519293506000926001600160a01b03909216916370a0823191602480820192602092909190829003018186803b158015610dd057600080fd5b505afa158015610de4573d6000803e3d6000fd5b505050506040513d6020811015610dfa57600080fd5b505190506000610e13836001600160701b038716611c1c565b90506000610e2a836001600160701b038716611c1c565b90506000610e388787611f3b565b6000549091508061100f5760055460408051637cd07e4760e01b815290516000926001600160a01b031691637cd07e47916004808301926020929190829003018186803b158015610e8857600080fd5b505afa158015610e9c573d6000803e3d6000fd5b505050506040513d6020811015610eb257600080fd5b50519050336001600160a01b0382161415610f8d57806001600160a01b03166340dc0e376040518163ffffffff1660e01b815260040160206040518083038186803b158015610f0057600080fd5b505afa158015610f14573d6000803e3d6000fd5b505050506040513d6020811015610f2a57600080fd5b505199508915801590610f3f57506000198a14155b610f88576040805162461bcd60e51b81526020600482015260156024820152744261642064657369726564206c697175696469747960581b604482015290519081900360640190fd5b611009565b6001600160a01b03811615610fe2576040805162461bcd60e51b815260206004820152601660248201527526bab9ba103737ba103430bb329036b4b3b930ba37b960511b604482015290519081900360640190fd5b610ffa6103e86109ce610ff58888611bb9565b61207b565b995061100960006103e86120cd565b50611052565b61104f6001600160701b0389166110268684611bb9565b8161102d57fe5b046001600160701b0389166110428685611bb9565b8161104957fe5b04612157565b98505b600089116110915760405162461bcd60e51b815260040180806020018281038252602881526020018061231a6028913960400191505060405180910390fd5b61109b8a8a6120cd565b6110a786868a8a611c6c565b81156110d1576008546110cd906001600160701b0380821691600160701b900416611bb9565b600b555b6040805185815260208101859052815133927f4c209b5fc8ad50758f13e2e1088ba56a560dff690a1c6fef26394f4c03821c4f928290030190a250506001600c5550949695505050505050565b60016020526000908152604090205481565b600b5481565b60046020526000908152604090205481565b600080600c54600114611196576040805162461bcd60e51b8152602060048201526011602482015270155b9a5cddd85c158c8e881313d0d2d151607a1b604482015290519081900360640190fd5b6000600c819055806111a6610af9565b50600654600754604080516370a0823160e01b815230600482015290519496509294506001600160a01b039182169391169160009184916370a08231916024808301926020929190829003018186803b15801561120257600080fd5b505afa158015611216573d6000803e3d6000fd5b505050506040513d602081101561122c57600080fd5b5051604080516370a0823160e01b815230600482015290519192506000916001600160a01b038516916370a08231916024808301926020929190829003018186803b15801561127a57600080fd5b505afa15801561128e573d6000803e3d6000fd5b505050506040513d60208110156112a457600080fd5b5051306000908152600160205260408120549192506112c38888611f3b565b600054909150806112d48487611bb9565b816112db57fe5b049a50806112e98486611bb9565b816112f057fe5b04995060008b118015611303575060008a115b61133e5760405162461bcd60e51b81526004018080602001828103825260288152602001806122f26028913960400191505060405180910390fd5b611348308461216f565b611353878d8d611a1f565b61135e868d8c611a1f565b604080516370a0823160e01b815230600482015290516001600160a01b038916916370a08231916024808301926020929190829003018186803b1580156113a457600080fd5b505afa1580156113b8573d6000803e3d6000fd5b505050506040513d60208110156113ce57600080fd5b5051604080516370a0823160e01b815230600482015290519196506001600160a01b038816916370a0823191602480820192602092909190829003018186803b15801561141a57600080fd5b505afa15801561142e573d6000803e3d6000fd5b505050506040513d602081101561144457600080fd5b5051935061145485858b8b611c6c565b811561147e5760085461147a906001600160701b0380821691600160701b900416611bb9565b600b555b604080518c8152602081018c905281516001600160a01b038f169233927fdccd412f0b1252819cb1fd330b93224ca42612892bb3f4f789976e6d81936496929081900390910190a35050505050505050506001600c81905550915091565b604051806040016040528060038152602001620534c560ec1b81525081565b6000610b30338484611e8d565b6103e881565b600c54600114611559576040805162461bcd60e51b8152602060048201526011602482015270155b9a5cddd85c158c8e881313d0d2d151607a1b604482015290519081900360640190fd5b6000600c55600654600754600854604080516370a0823160e01b815230600482015290516001600160a01b03948516949093169261160292859287926115fd926001600160701b03169185916370a0823191602480820192602092909190829003018186803b1580156115cb57600080fd5b505afa1580156115df573d6000803e3d6000fd5b505050506040513d60208110156115f557600080fd5b505190611c1c565b611a1f565b61167681846115fd6008600e9054906101000a90046001600160701b03166001600160701b0316856001600160a01b03166370a08231306040518263ffffffff1660e01b815260040180826001600160a01b0316815260200191505060206040518083038186803b1580156115cb57600080fd5b50506001600c5550565b6005546001600160a01b031681565b6007546001600160a01b031681565b428410156116e8576040805162461bcd60e51b8152602060048201526012602482015271155b9a5cddd85c158c8e881156141254915160721b604482015290519081900360640190fd5b6003546001600160a01b0380891660008181526004602090815260408083208054600180820190925582517f6e71edae12b1b97f4d1f60370fef10105fa2faae0126114a169c64845d6126c98186015280840196909652958d166060860152608085018c905260a085019590955260c08085018b90528151808603909101815260e08501825280519083012061190160f01b6101008601526101028501969096526101228085019690965280518085039096018652610142840180825286519683019690962095839052610162840180825286905260ff89166101828501526101a284018890526101c28401879052519193926101e280820193601f1981019281900390910190855afa158015611803573d6000803e3d6000fd5b5050604051601f1901519150506001600160a01b038116158015906118395750886001600160a01b0316816001600160a01b0316145b61188a576040805162461bcd60e51b815260206004820152601c60248201527f556e697377617056323a20494e56414c49445f5349474e415455524500000000604482015290519081900360640190fd5b611895898989611e2b565b505050505050505050565b600260209081526000928352604080842090915290825290205481565b600c54600114611908576040805162461bcd60e51b8152602060048201526011602482015270155b9a5cddd85c158c8e881313d0d2d151607a1b604482015290519081900360640190fd5b6000600c55600654604080516370a0823160e01b81523060048201529051611a18926001600160a01b0316916370a08231916024808301926020929190829003018186803b15801561195957600080fd5b505afa15801561196d573d6000803e3d6000fd5b505050506040513d602081101561198357600080fd5b5051600754604080516370a0823160e01b815230600482015290516001600160a01b03909216916370a0823191602480820192602092909190829003018186803b1580156119d057600080fd5b505afa1580156119e4573d6000803e3d6000fd5b505050506040513d60208110156119fa57600080fd5b50516008546001600160701b0380821691600160701b900416611c6c565b6001600c55565b604080518082018252601981527f7472616e7366657228616464726573732c75696e74323536290000000000000060209182015281516001600160a01b0385811660248301526044808301869052845180840390910181526064909201845291810180516001600160e01b031663a9059cbb60e01b1781529251815160009460609489169392918291908083835b60208310611acc5780518252601f199092019160209182019101611aad565b6001836020036101000a0380198251168184511680821785525050505050509050019150506000604051808303816000865af19150503d8060008114611b2e576040519150601f19603f3d011682016040523d82523d6000602084013e611b33565b606091505b5091509150818015611b61575080511580611b615750808060200190516020811015611b5e57600080fd5b50515b611bb2576040805162461bcd60e51b815260206004820152601a60248201527f556e697377617056323a205452414e534645525f4641494c4544000000000000604482015290519081900360640190fd5b5050505050565b6000811580611bd457505080820282828281611bd157fe5b04145b610b34576040805162461bcd60e51b815260206004820152601460248201527364732d6d6174682d6d756c2d6f766572666c6f7760601b604482015290519081900360640190fd5b80820382811115610b34576040805162461bcd60e51b815260206004820152601560248201527464732d6d6174682d7375622d756e646572666c6f7760581b604482015290519081900360640190fd5b6001600160701b038411801590611c8a57506001600160701b038311155b611cd1576040805162461bcd60e51b8152602060048201526013602482015272556e697377617056323a204f564552464c4f5760681b604482015290519081900360640190fd5b60085463ffffffff42811691600160e01b90048116820390811615801590611d0157506001600160701b03841615155b8015611d1557506001600160701b03831615155b15611d80578063ffffffff16611d3d85611d2e86612201565b6001600160e01b031690612213565b600980546001600160e01b03929092169290920201905563ffffffff8116611d6884611d2e87612201565b600a80546001600160e01b0392909216929092020190555b600880546dffffffffffffffffffffffffffff19166001600160701b03888116919091176dffffffffffffffffffffffffffff60701b1916600160701b8883168102919091176001600160e01b0316600160e01b63ffffffff871602179283905560408051848416815291909304909116602082015281517f1c411e9a96e071241c2f21f7726b17ae89e3cab4c78be50e062b03a9fffbbad1929181900390910190a1505050505050565b6001600160a01b03808416600081815260026020908152604080832094871680845294825291829020859055815185815291517f8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b9259281900390910190a3505050565b6001600160a01b038316600090815260016020526040902054611eb09082611c1c565b6001600160a01b038085166000908152600160205260408082209390935590841681522054611edf9082612238565b6001600160a01b0380841660008181526001602090815260409182902094909455805185815290519193928716927fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef92918290030190a3505050565b600080600560009054906101000a90046001600160a01b03166001600160a01b031663017e7e586040518163ffffffff1660e01b815260040160206040518083038186803b158015611f8c57600080fd5b505afa158015611fa0573d6000803e3d6000fd5b505050506040513d6020811015611fb657600080fd5b5051600b546001600160a01b038216158015945091925090612067578015612062576000611ff3610ff56001600160701b03888116908816611bb9565b905060006120008361207b565b90508082111561205f5760006120226120198484611c1c565b60005490611bb9565b9050600061203b83612035866005611bb9565b90612238565b9050600081838161204857fe5b049050801561205b5761205b87826120cd565b5050505b50505b612073565b8015612073576000600b555b505092915050565b600060038211156120be575080600160028204015b818110156120b8578091506002818285816120a757fe5b0401816120b057fe5b049050612090565b506120c8565b81156120c8575060015b919050565b6000546120da9082612238565b60009081556001600160a01b0383168152600160205260409020546120ff9082612238565b6001600160a01b03831660008181526001602090815260408083209490945583518581529351929391927fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef9281900390910190a35050565b60008183106121665781612168565b825b9392505050565b6001600160a01b0382166000908152600160205260409020546121929082611c1c565b6001600160a01b038316600090815260016020526040812091909155546121b99082611c1c565b60009081556040805183815290516001600160a01b038516917fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef919081900360200190a35050565b6001600160701b0316600160701b0290565b60006001600160701b0382166001600160e01b0384168161223057fe5b049392505050565b80820182811015610b34576040805162461bcd60e51b815260206004820152601460248201527364732d6d6174682d6164642d6f766572666c6f7760601b604482015290519081900360640190fdfe556e697377617056323a20494e53554646494349454e545f4f55545055545f414d4f554e54556e697377617056323a20494e53554646494349454e545f494e5055545f414d4f554e54556e697377617056323a20494e53554646494349454e545f4c4951554944495459556e697377617056323a20494e53554646494349454e545f4c49515549444954595f4255524e4544556e697377617056323a20494e53554646494349454e545f4c49515549444954595f4d494e544544a2646970667358221220713a8bf21df06433f34b5c9abf186abb737e72524583bdf420105a289791e24864736f6c634300060c0033a26469706673582212209c1e46967e61d91a65487ad45d080a227969fffa0564957df8e023b202f4d62a64736f6c634300060c0033000000000000000000000000f942dba4159cb61f8ad88ca4a83f5204e8f4a6bd"""
 
+
 # https://dev.sushi.com/sushiswap/contracts#sushiv2factory
 _SUSHI_V2_INIT_CODE_HASH = "e18a34eb0e04b04f7a0ac29a6e80748dca96319b42c54d679cb821dca90c6303"
 
 
 _GOOD_TRANSFER_SIGNATURES = (
     # https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/IERC20.sol#L75
     "Transfer(address,address,uint)",
```

### Comparing `web3-ethereum-defi-0.8/eth_defi/uniswap_v2/fees.py` & `web3-ethereum-defi-0.9/eth_defi/uniswap_v2/fees.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 `Mostly lifted from Uniswap-v2-py MIT licensed by Asynctomatic <https://github.com/nosofa/uniswap-v2-py>`_.
 """
 
 from decimal import Decimal
 from typing import List, Optional
 
 from eth_typing import HexAddress
-from web3 import Web3
+
 from web3.contract import Contract
+from web3.exceptions import BadFunctionCallOutput
 
 from eth_defi.token import fetch_erc20_details
-from eth_defi.uniswap_v2.deployment import UniswapV2Deployment
-from eth_defi.uniswap_v2.utils import pair_for, sort_tokens
+from eth_defi.uniswap_v2.deployment import UniswapV2Deployment, INIT_CODE_HASH_MISSING
+
+
+class BadReserves(Exception):
+    pass
 
 
 class UniswapV2FeeCalculator:
     """A helper class to estimate Uniswap fees."""
 
     def __init__(self, uniswap_v2: UniswapV2Deployment):
         self.deployment = uniswap_v2
@@ -29,21 +33,28 @@
 
         :param pair: Address of the pair.
         :return:
             - reserve_0 - Amount of token_0 in the contract.
             - reserve_1 - Amount of token_1 in the contract.
             - liquidity - Unix timestamp of the block containing the last pair interaction.
         """
+
+        assert self.deployment.init_code_hash is not None, "Init hash not set"
+        assert self.deployment.init_code_hash != INIT_CODE_HASH_MISSING, "You need to set init hash to use get_reserves()"
+
         assert token_a.startswith("0x")
         assert token_b.startswith("0x")
-        (token0, token1) = sort_tokens(token_a, token_b)
-        pair_contract = self.deployment.PairContract(
-            address=Web3.toChecksumAddress(pair_for(self.deployment.factory.address, token_a, token_b, self.deployment.init_code_hash)),
-        )
-        reserve = pair_contract.functions.getReserves().call()
+
+        # (token0, token1) = sort_tokens(token_a, token_b)
+        pair_address, token0, token1 = self.deployment.pair_for(token_a, token_b)
+        pair_contract = self.deployment.PairContract(pair_address)
+        try:
+            reserve = pair_contract.functions.getReserves().call()
+        except BadFunctionCallOutput as e:
+            raise BadReserves(f"Could not get reserves, bad pair contract {pair_address}, init hash {self.deployment.init_code_hash}, token_a {token_a}, token_b {token_b}?") from e
         return reserve if token0 == token_a else [reserve[1], reserve[0], reserve[2]]
 
     def get_amounts_out(
         self,
         amount_in: int,
         path: List[HexAddress],
         *,
@@ -100,14 +111,15 @@
         for index, (p0, p1) in enumerate(pairs):
             r = self.get_reserves(p0, p1)
 
             # since we care only about the first amount in, apply slippage to only first pair calculation
             _slippage = 0
             if index == 0:
                 _slippage = slippage
+
             current_amount = self.get_amount_in(current_amount, r[0], r[1], fee=fee, slippage=_slippage)
 
             amounts.insert(0, current_amount)
 
         return amounts
 
     @staticmethod
@@ -169,14 +181,16 @@
     quantity: int,
     *,
     fee: int = 30,
     slippage: float = 0,
 ) -> int:
     """Estimate how many tokens we are going to receive when doing a buy.
 
+    Good for doing a price impact calculations.
+
     Calls the on-chain contract to get the current liquidity and estimates the
     the price based on it.
 
     Example:
 
     .. code-block:: python
 
@@ -359,17 +373,16 @@
     :param quote_token: Quote token of the trading pair
     :param fee: Trading fee express in bps, default = 30 bps (0.3%)
     :param slippage: Slippage express in bps
     :return: Expected quote token amount to receive
     :raise TokenDetailError: If we have an issue with ERC-20 contracts
     """
     web3 = uniswap.web3
-    base = fetch_erc20_details(web3, base_token_address, raise_on_error=False)
     quote = fetch_erc20_details(web3, quote_token_address, raise_on_error=False)
-    quantity_raw = base.convert_to_raw(quantity)
+    quantity_raw = quote.convert_to_raw(quantity)
     fee_helper = UniswapV2FeeCalculator(uniswap)
 
     if intermediate_token_address:
         path = [quote_token_address, intermediate_token_address, base_token_address]
     else:
         path = [quote_token_address, base_token_address]
     amounts = fee_helper.get_amounts_in(quantity_raw, path, fee=fee, slippage=slippage)
@@ -412,7 +425,129 @@
         path = [base_token_address, intermediate_token_address, quote_token_address]
     else:
         path = [base_token_address, quote_token_address]
     amounts = fee_helper.get_amounts_out(quantity_raw, path, fee=fee, slippage=slippage)
 
     out_raw = amounts[-1]
     return quote.convert_to_decimals(out_raw)
+
+
+def estimate_buy_received_amount_raw(
+    uniswap: UniswapV2Deployment,
+    base_token_address: HexAddress,
+    quote_token_address: HexAddress,
+    quantity_raw: Decimal,
+    *,
+    fee: int = 30,
+    slippage: float = 0,
+    intermediate_token_address: Optional[HexAddress] = None,
+) -> int:
+    """Estimate how much we receive for a certain cash amount.
+
+    Example:
+
+    .. code-block:: python
+
+        # Create the trading pair and add initial liquidity
+        deploy_trading_pair(
+            web3,
+            deployer,
+            uniswap_v2,
+            weth,
+            usdc,
+            1_000 * 10**18,  # 1000 ETH liquidity
+            1_700_000 * 10**18,  # 1.7M USDC liquidity
+        )
+
+        # Estimate the price of buying 1650 USDC worth of ETH
+        eth_received = estimate_buy_received_amount_raw(
+            uniswap_v2,
+            weth.address,
+            usdc.address,
+            1650 * 10**18,
+        )
+
+        assert eth_received / (10**18) == pytest.approx(0.9667409780905836)
+
+        # Calculate price of ETH as $ for our purchase
+        price = (1650*10**18) / eth_received
+        assert price == pytest.approx(Decimal(1706.7653460381143))
+
+    :param quantity: How much of the base token we want to buy
+    :param uniswap: Uniswap v2 deployment
+    :param base_token: Base token of the trading pair
+    :param quote_token: Quote token of the trading pair
+    :param fee: Trading fee express in bps, default = 30 bps (0.3%)
+    :param slippage: Slippage express in bps
+    :return: Expected quote token amount to receive
+    :raise TokenDetailError: If we have an issue with ERC-20 contracts
+    """
+    fee_helper = UniswapV2FeeCalculator(uniswap)
+
+    if intermediate_token_address:
+        path = [quote_token_address, intermediate_token_address, base_token_address]
+    else:
+        path = [quote_token_address, base_token_address]
+
+    # We will receive equal number of amounts as there are items in the path
+    amounts = fee_helper.get_amounts_out(quantity_raw, path, fee=fee, slippage=slippage)
+    return amounts[-1]
+
+
+def estimate_sell_received_amount_raw(
+    uniswap: UniswapV2Deployment,
+    base_token_address: HexAddress,
+    quote_token_address: HexAddress,
+    quantity_raw: Decimal,
+    *,
+    fee: int = 30,
+    slippage: float = 0,
+    intermediate_token_address: Optional[HexAddress] = None,
+) -> int:
+    """Estimate how much cash we receive for a certain quantity of tokens sold.
+
+    Example:
+
+    .. code-block:: python
+
+        deploy_trading_pair(
+            web3,
+            deployer,
+            uniswap_v2,
+            weth,
+            usdc,
+            1_000 * 10**18,  # 1000 ETH liquidity
+            1_700_000 * 10**18,  # 1.7M USDC liquidity
+        )
+
+        # Sell 50 ETH
+        usdc_received = estimate_sell_received_amount_raw(
+            uniswap_v2,
+            weth.address,
+            usdc.address,
+            50 * 10**18,
+        )
+
+        usdc_received_decimals = usdc_received / 10**18
+        assert usdc_received_decimals == pytest.approx(80721.05538886508)
+
+        # Calculate price of ETH as $ for our purchase
+        price = usdc_received / (50*10**18)
+        assert price == pytest.approx(Decimal(1614.4211077773016))
+
+    :param quantity: How much of the base token we want to buy
+    :param uniswap: Uniswap v2 deployment
+    :param base_token: Base token of the trading pair
+    :param quote_token: Quote token of the trading pair
+    :param fee: Trading fee express in bps, default = 30 bps (0.3%)
+    :param slippage: Slippage express in bps
+    :return: Expected quote token amount to receive
+    :raise TokenDetailError: If we have an issue with ERC-20 contracts
+    """
+    fee_helper = UniswapV2FeeCalculator(uniswap)
+
+    if intermediate_token_address:
+        path = (base_token_address, intermediate_token_address, quote_token_address)
+    else:
+        path = (base_token_address, quote_token_address)
+    amounts = fee_helper.get_amounts_out(quantity_raw, path, fee=fee, slippage=slippage)
+    return amounts[-1]
```

### Comparing `web3-ethereum-defi-0.8/eth_defi/uniswap_v2/liquidity.py` & `web3-ethereum-defi-0.9/eth_defi/uniswap_v2/liquidity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Liquidity measuring."""
 from dataclasses import dataclass
-from typing import Union, Tuple
+from typing import Union
 
 from eth_typing import HexAddress
 from web3 import Web3
 from web3.contract import Contract
 
 from eth_defi.abi import get_deployed_contract
 
@@ -93,8 +93,7 @@
         pair,
         token0,
         token1,
         reserve_result[0],
         reserve_result[1],
         reserve_result[2],
     )
-
```

### Comparing `web3-ethereum-defi-0.8/eth_defi/uniswap_v2/swap.py` & `web3-ethereum-defi-0.9/eth_defi/uniswap_v2/swap.py`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/uniswap_v2/token_tax.py` & `web3-ethereum-defi-0.9/eth_defi/uniswap_v2/token_tax.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,20 +27,22 @@
 
 class TransferFromError(Exception):
     """The token is likely broken.
 
     See KICK on Ethereum mainnet.
     """
 
+
 class OutOfGasDuringTransfer(Exception):
     """The token is likely some sort of ponzi with restricted transfer.
 
     See WETH-CGT on Ethereum mainnet.
     """
 
+
 class OutOfGasDuringSell(Exception):
     """The token is likely some sort of ponzi with restricted transfer.
 
     See WETH-DEXE on Ethereum mainnet: 0xde4ee8057785a7e8e800db58f9784845a5c2cbd6
     """
 
 
@@ -87,16 +89,16 @@
         quote_token: HexAddress,
         buy_account: HexAddress,
         sell_account: HexAddress,
         buy_amount: float,
         approve=True,
         quote_token_details: Optional[TokenDetails] = None,
         base_token_details: Optional[TokenDetails] = None,
-        gas_limit: Optional[int]=None,
-        gas_price: Optional[int]=None,
+        gas_limit: Optional[int] = None,
+        gas_price: Optional[int] = None,
 ) -> TokenTaxInfo:
     """Estimates different token taxes for a token by running Ganache simulations for it.
 
     :param uniswap:
         Uniswap deployment on a Ganache mainnet fork.
         Set up prior calling this function.
         See `ganache.py` and `test_ganache.py` for more details.
```

### Comparing `web3-ethereum-defi-0.8/eth_defi/uniswap_v2/utils.py` & `web3-ethereum-defi-0.9/eth_defi/uniswap_v2/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 #: Ethereum 0x000000000 addresss
 ZERO_ADDRESS = Web3.toHex(0x0)
 
 
 def sort_tokens(token_a: HexAddress, token_b: HexAddress) -> Tuple[HexAddress, HexAddress]:
     """Put lower address first, as Uniswap wants."""
-    assert token_a != token_b
+    assert token_a != token_b, f"Received bad token pair {token_a}:{token_b}"
     (token_0, token_1) = (token_a, token_b) if int(token_a, 16) < int(token_b, 16) else (token_b, token_a)
     assert token_0 != ZERO_ADDRESS
     return token_0, token_1
 
 
 # Liften from uniswap-v2-py by Asynctomatic
 def pair_for(factory: HexAddress, token_a: HexAddress, token_b: HexAddress, magical_hash: HexStr) -> HexAddress:
@@ -26,11 +26,13 @@
     :param factory: Factory contract address
     :param token_a: Base token
     :param token_b: Quote token
     :param magical_hash: Init code hash of the Uniswap instance. Set None to use the default Sushiswap hash.
     :return: Pair contract address
     """
     prefix = Web3.toHex(hexstr="ff")
+    token_a = Web3.toChecksumAddress(token_a)
+    token_b = Web3.toChecksumAddress(token_b)
     encoded_tokens = Web3.solidityKeccak(["address", "address"], sort_tokens(token_a, token_b))
     suffix = Web3.toHex(hexstr=magical_hash)
     raw = Web3.solidityKeccak(["bytes", "address", "bytes", "bytes"], [prefix, factory, encoded_tokens, suffix])
     return Web3.toChecksumAddress(Web3.toHex(raw)[-40:])
```

### Comparing `web3-ethereum-defi-0.8/eth_defi/uniswap_v3/constants.py` & `web3-ethereum-defi-0.9/eth_defi/uniswap_v3/constants.py`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/uniswap_v3/deployment.py` & `web3-ethereum-defi-0.9/eth_defi/uniswap_v3/deployment.py`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/uniswap_v3/utils.py` & `web3-ethereum-defi-0.9/eth_defi/uniswap_v3/utils.py`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/eth_defi/utils.py` & `web3-ethereum-defi-0.9/eth_defi/utils.py`

 * *Files identical despite different names*

### Comparing `web3-ethereum-defi-0.8/pyproject.toml` & `web3-ethereum-defi-0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "web3-ethereum-defi"
-version = "0.8"
-description = "Web3 Ethereum DeFi toolkit for smart contracts, Ethereum JSON-RPC utilities, Uniswap, PancakeSwap, wallets and automated test suites."
+version = "0.9"
+description = "Web3-Ethereum-DeFi is a library for smart contracts, DeFi trading (Uniswap, PancakeSwap), Ethereum JSON-RPC, EVM transactions and automated test suites."
 authors = ["Mikko Ohtamaa <mikko@tradingstrategy.ai>"]
 license = "MIT"
 homepage = "https://tradingstrategy.ai"
 repository = "https://github.com/tradingstrategy-ai/web3-ethereum-defi"
 readme = "README.md"
 keywords = ["ethereum", "cryptocurrency", "uniswap", "erc-20", "pancakeswap", "sushiswap", "polygon", "web3", "blockchain"]
 packages = [
@@ -16,14 +16,17 @@
 python = "^3.8"
 web3 = {extras = ["tester"], version = "^5.28.0"}
 Sphinx = {version = "^4.4.0", optional = true}
 sphinx-rtd-theme = {version = "^1.0.0", optional = true}
 sphinx-sitemap = {version = "^2.2.0", optional = true}
 sphinx-autodoc-typehints = {version = "^1.16.0", extras = ["docs"], optional = true}
 psutil = "^5.9.0"
+eth-bloom = "^1.0.4"
+ujson = "^5.2.0"
+futureproof = "^0.3.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-sitemap = "^2.2.0"
 ipdb = "^0.13.9"
 black = "^22.1.0"
```

### Comparing `web3-ethereum-defi-0.8/setup.py` & `web3-ethereum-defi-0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['eth_defi', 'eth_defi.uniswap_v2', 'eth_defi.uniswap_v3']
+['eth_defi',
+ 'eth_defi.event_reader',
+ 'eth_defi.uniswap_v2',
+ 'eth_defi.uniswap_v3']
 
 package_data = \
 {'': ['*'], 'eth_defi': ['abi/*', 'abi/uniswap_v3/*']}
 
 install_requires = \
-['psutil>=5.9.0,<6.0.0', 'web3[tester]>=5.28.0,<6.0.0']
+['eth-bloom>=1.0.4,<2.0.0',
+ 'futureproof>=0.3.1,<0.4.0',
+ 'psutil>=5.9.0,<6.0.0',
+ 'ujson>=5.2.0,<6.0.0',
+ 'web3[tester]>=5.28.0,<6.0.0']
 
 extras_require = \
 {'docs': ['Sphinx>=4.4.0,<5.0.0',
           'sphinx-rtd-theme>=1.0.0,<2.0.0',
           'sphinx-sitemap>=2.2.0,<3.0.0',
           'sphinx-autodoc-typehints[docs]>=1.16.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'web3-ethereum-defi',
-    'version': '0.8',
-    'description': 'Web3 Ethereum DeFi toolkit for smart contracts, Ethereum JSON-RPC utilities, Uniswap, PancakeSwap, wallets and automated test suites.',
-    'long_description': '[![PyPI version](https://badge.fury.io/py/web3-ethereum-defi.svg)](https://badge.fury.io/py/web3-ethereum-defi)\n\n[![Automated test suite](https://github.com/tradingstrategy-ai/web3-ethereum-defi/actions/workflows/test.yml/badge.svg)](https://github.com/tradingstrategy-ai/web3-ethereum-defi/actions/workflows/test.yml)\n\n[![Documentation Status](https://readthedocs.org/projects/web3-ethereum-defi/badge/?version=latest)](https://web3-ethereum-defi.readthedocs.io/en/latest/?badge=latest)\n\n# Web3 Ethereum Defi\n\nThis project contains common Ethereum smart contracts and utilities, \nfor trading, wallets,automated test suites and backend integrations for EVM based blockchains.  \n\n* [Features](#features)\n* [Precompiled ABI file distribution](#precompiled-abi-file-distribution)\n* [Python usage](#python-usage)\n   * [Prerequisites](#prerequisites)\n   * [ERC-20 token example](#erc-20-token-example)\n   * [Uniswap v2 trade example](#uniswap-v2-trade-example)\n   * [Uniswap v2 price estimation example](#uniswap-v2-price-estimation-example)\n   * [How to use the library in your Python project](#how-to-use-the-library-in-your-python-project)\n* [Development](#development)\n   * [Build requirements](#build-requirements)\n   * [Make](#make)\n* [Version history](#version-history)\n* [Discord](#discord)\n* [Notes](#notes)\n* [History](#history)\n* [License](#license)\n\n![Pepe chooses Web3 Ethereum DeFi and Python](https://raw.githubusercontent.com/tradingstrategy-ai/web3-ethereum-defi/master/docs/source/_static/pepe.jpg)\n\n**Pepe chooses web3-ethereum-defi and Python**.\n\n# Features\n\nFeatures include \n\n* [Made for 99% developers](https://future.a16z.com/software-development-building-for-99-developers/)\n* [High-quality API documentation](https://web3-ethereum-defi.readthedocs.io/)\n* [Fully type hinted](https://web3-ethereum-defi.readthedocs.io/) for good developer experience\n* [ERC-20 token issuance and manipulation](https://web3-ethereum-defi.readthedocs.io/en/latest/_autosummary/eth_defi.token.html#module-eth_defi.token)\n* [Uniswap v2 tools](https://github.com/sushiswap/sushiswap): deployment, trading, price estimation for Sushiswap, PancakeSwape, QuickSwap, Trader Joe, others\n* [Parallel transaction execution](https://web3-ethereum-defi.readthedocs.io/en/latest/_autosummary/eth_defi.txmonitor.html)\n* [Mainnet forking with ganache-cli](https://web3-ethereum-defi.readthedocs.io/en/latest/_autosummary/eth_defi.ganache.fork_network.html#eth_defi.ganache.fork_network)\n* As opposite to slower and messier [mainnet forking workflows](https://www.quicknode.com/guides/web3-sdks/how-to-fork-ethereum-blockchain-with-ganache), \nthis project aims to explicit clean deployments and very fast test execution.\n* (More integrations to come)\n\n# Precompiled ABI file distribution\n\nThe project provides a precompiled smart contract bundle, including ABI files, full source\nand debug maps, to make deploying test instances trivial.\n\nThis package primarly supports Python, Web3.p3 and Brownie developers.\nFor other programming languages and frameworks,\nyou can [find precompiled Solidity smart contracts in abi folder](https://github.com/tradingstrategy-ai/web3-ethereum-defi/tree/master/eth_defi/abi).\n\nThese files are good to go with any framework:\n* Web3.js\n* Ethers.js\n* Hardhat\n* Truffle\n* Web3j\n\nEach JSON file has `abi` and `bytecode` keys you need to deploy a contract.\n\nJust download and embed in your project. \nThe compiled source code files are mixture of MIT and GPL v2 license.\n\n# Python usage\n\nThe Python support is available as `web3-ethereum-defi` Python package.\n\nThe package depends only on [web3.py](github.com/ethereum/web3.py) and not others, like [Brownie](https://eth-brownie.readthedocs.io/).\nIt grabs popular ABI files with their bytecode and compilation artifacts so that the contracts\nare easily deployable on any Ethereum tester interface. No Ganache is needed and everything\ncan be executed on faster [eth-tester enginer](https://github.com/ethereum/eth-tester).\n\nUnlike Brownie, which is a framework, `web3-ethereum-defi` is a library. It is designed\nto be included in any other Python application and you can only use bits of its that you need.\nThere are no expectations on configuration files or folder structure.\n\n[Read the full API documentation](High-quality API documentation](https://web3-ethereum-defi.readthedocs.io/)).\nFor code examples please see below.\n\n## Prerequisites\n\n* [Proficient in Python programming](https://wiki.python.org/moin/BeginnersGuide)\n* [Understanding of Web3.py library](https://web3py.readthedocs.io/en/stable/) \n* [pytest basics](https://docs.pytest.org/)\n\n## ERC-20 token example\n\nTo use the package to deploy a simple ERC-20 token in [pytest](https://docs.pytest.org/) testing:\n\n```python\nimport pytest\nfrom web3 import Web3, EthereumTesterProvider\n\nfrom eth_defi.token import create_token\n\n\n@pytest.fixture\ndef tester_provider():\n    return EthereumTesterProvider()\n\n\n@pytest.fixture\ndef eth_tester(tester_provider):\n    return tester_provider.ethereum_tester\n\n\n@pytest.fixture\ndef web3(tester_provider):\n    return Web3(tester_provider)\n\n\n@pytest.fixture()\ndef deployer(web3) -> str:\n    """Deploy account."""\n    return web3.eth.accounts[0]\n\n\n@pytest.fixture()\ndef user_1(web3) -> str:\n    """User account."""\n    return web3.eth.accounts[1]\n\n\n@pytest.fixture()\ndef user_2(web3) -> str:\n    """User account."""\n    return web3.eth.accounts[2]\n\n\ndef test_deploy_token(web3: Web3, deployer: str):\n    """Deploy mock ERC-20."""\n    token = create_token(web3, deployer, "Hentai books token", "HENTAI", 100_000 * 10**18)\n    assert token.functions.name().call() == "Hentai books token"\n    assert token.functions.symbol().call() == "HENTAI"\n    assert token.functions.totalSupply().call() == 100_000 * 10**18\n    assert token.functions.decimals().call() == 18\n\n\ndef test_tranfer_tokens_between_users(web3: Web3, deployer: str, user_1: str, user_2: str):\n    """Transfer tokens between users."""\n    token = create_token(web3, deployer, "Telos EVM rocks", "TELOS", 100_000 * 10**18)\n\n    # Move 10 tokens from deployer to user1\n    token.functions.transfer(user_1, 10 * 10**18).transact({"from": deployer})\n    assert token.functions.balanceOf(user_1).call() == 10 * 10**18\n\n    # Move 10 tokens from deployer to user1\n    token.functions.transfer(user_2, 6 * 10**18).transact({"from": user_1})\n    assert token.functions.balanceOf(user_1).call() == 4 * 10**18\n    assert token.functions.balanceOf(user_2).call() == 6 * 10**18\n```\n\n[See full example](https://github.com/tradingstrategy-ai/web3-ethereum-defi/blob/master/tests/test_token.py).\n\n[For more information how to user Web3.py in testing, see Web3.py documentation](https://web3py.readthedocs.io/en/stable/examples.html#contract-unit-tests-in-python).\n\n## Uniswap v2 trade example\n\n```python\nimport pytest\nfrom web3 import Web3\nfrom web3.contract import Contract\n\nfrom eth_defi.uniswap_v2.deployment import UniswapV2Deployment, deploy_trading_pair, FOREVER_DEADLINE\n\n\ndef test_swap(web3: Web3, deployer: str, user_1: str, uniswap_v2: UniswapV2Deployment, weth: Contract, usdc: Contract):\n    """User buys WETH on Uniswap v2 using mock USDC."""\n\n    # Create the trading pair and add initial liquidity\n    deploy_trading_pair(\n        web3,\n        deployer,\n        uniswap_v2,\n        weth,\n        usdc,\n        10 * 10**18,  # 10 ETH liquidity\n        17_000 * 10**18,  # 17000 USDC liquidity\n    )\n\n    router = uniswap_v2.router\n\n    # Give user_1 500 dollars to buy ETH and approve it on the router\n    usdc_amount_to_pay = 500 * 10**18\n    usdc.functions.transfer(user_1, usdc_amount_to_pay).transact({"from": deployer})\n    usdc.functions.approve(router.address, usdc_amount_to_pay).transact({"from": user_1})\n\n    # Perform a swap USDC->WETH\n    path = [usdc.address, weth.address]  # Path tell how the swap is routed\n    # https://docs.uniswap.org/protocol/V2/reference/smart-contracts/router-02#swapexacttokensfortokens\n    router.functions.swapExactTokensForTokens(\n        usdc_amount_to_pay,\n        0,\n        path,\n        user_1,\n        FOREVER_DEADLINE,\n    ).transact({\n        "from": user_1\n    })\n\n    # Check the user_1 received ~0.284 ethers\n    assert weth.functions.balanceOf(user_1).call() / 1e18 == pytest.approx(0.28488156127668085)\n```\n\n[See the full example](https://github.com/tradingstrategy-ai/web3-ethereum-defi/blob/master/tests/test_uniswap_v2_pair.py).\n\n## Uniswap v2 price estimation example\n\n```python\n# Create the trading pair and add initial liquidity\ndeploy_trading_pair(\n    web3,\n    deployer,\n    uniswap_v2,\n    weth,\n    usdc,\n    1_000 * 10**18,  # 1000 ETH liquidity\n    1_700_000 * 10**18,  # 1.7M USDC liquidity\n)\n\n# Estimate the price of buying 1 ETH\nusdc_per_eth = estimate_buy_price_decimals(\n    uniswap_v2,\n    weth.address,\n    usdc.address,\n    Decimal(1.0),\n)\nassert usdc_per_eth == pytest.approx(Decimal(1706.82216820632059904))\n```\n\n[See full example](https://github.com/tradingstrategy-ai/web3-ethereum-defi/blob/34a9e1b948a4ef5a620ee520b568c0fd27c75457/tests/test_uniswap_v2_pair.py#L243).\n\n## How to use the library in your Python project\n\nAdd `web3-ethereum-defi` as a development dependency:\n\nUsing [Poetry](https://python-poetry.org/):\n\n```shell\npoetry add -D web3-ethereum-defi\n```\n\n# Development and contributing\n\n[Read development instructions](https://web3-ethereum-defi.readthedocs.io/development.html).\n\n# Version history\n\n- [Read changelog](https://github.com/tradingstrategy-ai/web3-ethereum-defi/blob/master/CHANGELOG.md).\n- [See releases](https://pypi.org/project/web3-ethereum-defi/#history).\n\n# Discord\n\n[Join Discord for any questions](https://tradingstrategy.ai/community).\n\n# Notes\n\nCurrently there is no [Brownie](https://eth-brownie.readthedocs.io/) support.\nTo support Brownie, one would need to figure out how to import an existing Hardhat\nbased project (Sushiswap) to Brownie project format.\n\n# History\n\n[Originally created for Trading Strategy](https://tradingstrategy.ai). \n[Originally the package was known as eth-hentai](https://raw.githubusercontent.com/tradingstrategy-ai/web3-ethereum-defi/master/docs/source/_static/hentai_teacher_mikisugi_by_ilmaris_d6tjrn8-fullview.jpg).\n\n# License \n\nMIT\n',
+    'version': '0.9',
+    'description': 'Web3-Ethereum-DeFi is a library for smart contracts, DeFi trading (Uniswap, PancakeSwap), Ethereum JSON-RPC, EVM transactions and automated test suites.',
+    'long_description': '[![PyPI version](https://badge.fury.io/py/web3-ethereum-defi.svg)](https://badge.fury.io/py/web3-ethereum-defi)\n\n[![Automated test suite](https://github.com/tradingstrategy-ai/web3-ethereum-defi/actions/workflows/test.yml/badge.svg)](https://github.com/tradingstrategy-ai/web3-ethereum-defi/actions/workflows/test.yml)\n\n[![Documentation Status](https://readthedocs.org/projects/web3-ethereum-defi/badge/?version=latest)](https://web3-ethereum-defi.readthedocs.io/en/latest/?badge=latest)\n\n# Web3 Ethereum Defi\n\nThis project contains common Ethereum smart contracts and utilities, \nfor trading, wallets,automated test suites and backend integrations for EVM based blockchains.  \n\n* [Features](#features)\n* [Precompiled ABI file distribution](#precompiled-abi-file-distribution)\n* [Python usage](#python-usage)\n   * [Prerequisites](#prerequisites)\n   * [ERC-20 token example](#erc-20-token-example)\n   * [Uniswap v2 trade example](#uniswap-v2-trade-example)\n   * [Uniswap v2 price estimation example](#uniswap-v2-price-estimation-example)\n   * [How to use the library in your Python project](#how-to-use-the-library-in-your-python-project)\n* [Development](#development)\n   * [Build requirements](#build-requirements)\n   * [Make](#make)\n* [Version history](#version-history)\n* [Social media](#social-media)\n* [Notes](#notes)\n* [History](#history)\n* [License](#license)\n\n![Pepe chooses Web3 Ethereum DeFi and Python](https://raw.githubusercontent.com/tradingstrategy-ai/web3-ethereum-defi/master/docs/source/_static/pepe.jpg)\n\n**Pepe chooses web3-ethereum-defi and Python**.\n\n# Features\n\nFeatures include \n\n* [Made for 99% developers](https://future.a16z.com/software-development-building-for-99-developers/)\n* [High-quality API documentation](https://web3-ethereum-defi.readthedocs.io/)\n* [Fully type hinted](https://web3-ethereum-defi.readthedocs.io/) for good developer experience\n* [ERC-20 token issuance and manipulation](https://web3-ethereum-defi.readthedocs.io/en/latest/_autosummary/eth_defi.token.html#module-eth_defi.token)\n* [Uniswap v2 tools](https://github.com/sushiswap/sushiswap): deployment, trading, price estimation for Sushiswap, PancakeSwape, QuickSwap, Trader Joe, others\n* [Parallel transaction execution](https://web3-ethereum-defi.readthedocs.io/en/latest/_autosummary/eth_defi.txmonitor.html)\n* [Mainnet forking with ganache-cli](https://web3-ethereum-defi.readthedocs.io/en/latest/_autosummary/eth_defi.ganache.fork_network.html#eth_defi.ganache.fork_network)\n* As opposite to slower and messier [mainnet forking workflows](https://www.quicknode.com/guides/web3-sdks/how-to-fork-ethereum-blockchain-with-ganache), \nthis project aims to explicit clean deployments and very fast test execution.\n* (More integrations to come)\n\n# Precompiled ABI file distribution\n\nThe project provides a precompiled smart contract bundle, including ABI files, full source\nand debug maps, to make deploying test instances trivial.\n\nThis package primarly supports Python, Web3.p3 and Brownie developers.\nFor other programming languages and frameworks,\nyou can [find precompiled Solidity smart contracts in abi folder](https://github.com/tradingstrategy-ai/web3-ethereum-defi/tree/master/eth_defi/abi).\n\nThese files are good to go with any framework:\n* Web3.js\n* Ethers.js\n* Hardhat\n* Truffle\n* Web3j\n\nEach JSON file has `abi` and `bytecode` keys you need to deploy a contract.\n\nJust download and embed in your project. \nThe compiled source code files are mixture of MIT and GPL v2 license.\n\n# Python usage\n\nThe Python support is available as `web3-ethereum-defi` Python package.\n\nThe package depends only on [web3.py](github.com/ethereum/web3.py) and not others, like [Brownie](https://eth-brownie.readthedocs.io/).\nIt grabs popular ABI files with their bytecode and compilation artifacts so that the contracts\nare easily deployable on any Ethereum tester interface. No Ganache is needed and everything\ncan be executed on faster [eth-tester enginer](https://github.com/ethereum/eth-tester).\n\nUnlike Brownie, which is a framework, `web3-ethereum-defi` is a library. It is designed\nto be included in any other Python application and you can only use bits of its that you need.\nThere are no expectations on configuration files or folder structure.\n\n[Read the full API documentation](High-quality API documentation](https://web3-ethereum-defi.readthedocs.io/)).\nFor code examples please see below.\n\n## Prerequisites\n\n* [Proficient in Python programming](https://wiki.python.org/moin/BeginnersGuide)\n* [Understanding of Web3.py library](https://web3py.readthedocs.io/en/stable/) \n* [pytest basics](https://docs.pytest.org/)\n\n## ERC-20 token example\n\nTo use the package to deploy a simple ERC-20 token in [pytest](https://docs.pytest.org/) testing:\n\n```python\nimport pytest\nfrom web3 import Web3, EthereumTesterProvider\n\nfrom eth_defi.token import create_token\n\n\n@pytest.fixture\ndef tester_provider():\n    return EthereumTesterProvider()\n\n\n@pytest.fixture\ndef eth_tester(tester_provider):\n    return tester_provider.ethereum_tester\n\n\n@pytest.fixture\ndef web3(tester_provider):\n    return Web3(tester_provider)\n\n\n@pytest.fixture()\ndef deployer(web3) -> str:\n    """Deploy account."""\n    return web3.eth.accounts[0]\n\n\n@pytest.fixture()\ndef user_1(web3) -> str:\n    """User account."""\n    return web3.eth.accounts[1]\n\n\n@pytest.fixture()\ndef user_2(web3) -> str:\n    """User account."""\n    return web3.eth.accounts[2]\n\n\ndef test_deploy_token(web3: Web3, deployer: str):\n    """Deploy mock ERC-20."""\n    token = create_token(web3, deployer, "Hentai books token", "HENTAI", 100_000 * 10**18)\n    assert token.functions.name().call() == "Hentai books token"\n    assert token.functions.symbol().call() == "HENTAI"\n    assert token.functions.totalSupply().call() == 100_000 * 10**18\n    assert token.functions.decimals().call() == 18\n\n\ndef test_tranfer_tokens_between_users(web3: Web3, deployer: str, user_1: str, user_2: str):\n    """Transfer tokens between users."""\n    token = create_token(web3, deployer, "Telos EVM rocks", "TELOS", 100_000 * 10**18)\n\n    # Move 10 tokens from deployer to user1\n    token.functions.transfer(user_1, 10 * 10**18).transact({"from": deployer})\n    assert token.functions.balanceOf(user_1).call() == 10 * 10**18\n\n    # Move 10 tokens from deployer to user1\n    token.functions.transfer(user_2, 6 * 10**18).transact({"from": user_1})\n    assert token.functions.balanceOf(user_1).call() == 4 * 10**18\n    assert token.functions.balanceOf(user_2).call() == 6 * 10**18\n```\n\n[See full example](https://github.com/tradingstrategy-ai/web3-ethereum-defi/blob/master/tests/test_token.py).\n\n[For more information how to user Web3.py in testing, see Web3.py documentation](https://web3py.readthedocs.io/en/stable/examples.html#contract-unit-tests-in-python).\n\n## Uniswap v2 trade example\n\n```python\nimport pytest\nfrom web3 import Web3\nfrom web3.contract import Contract\n\nfrom eth_defi.uniswap_v2.deployment import UniswapV2Deployment, deploy_trading_pair, FOREVER_DEADLINE\n\n\ndef test_swap(web3: Web3, deployer: str, user_1: str, uniswap_v2: UniswapV2Deployment, weth: Contract, usdc: Contract):\n    """User buys WETH on Uniswap v2 using mock USDC."""\n\n    # Create the trading pair and add initial liquidity\n    deploy_trading_pair(\n        web3,\n        deployer,\n        uniswap_v2,\n        weth,\n        usdc,\n        10 * 10**18,  # 10 ETH liquidity\n        17_000 * 10**18,  # 17000 USDC liquidity\n    )\n\n    router = uniswap_v2.router\n\n    # Give user_1 500 dollars to buy ETH and approve it on the router\n    usdc_amount_to_pay = 500 * 10**18\n    usdc.functions.transfer(user_1, usdc_amount_to_pay).transact({"from": deployer})\n    usdc.functions.approve(router.address, usdc_amount_to_pay).transact({"from": user_1})\n\n    # Perform a swap USDC->WETH\n    path = [usdc.address, weth.address]  # Path tell how the swap is routed\n    # https://docs.uniswap.org/protocol/V2/reference/smart-contracts/router-02#swapexacttokensfortokens\n    router.functions.swapExactTokensForTokens(\n        usdc_amount_to_pay,\n        0,\n        path,\n        user_1,\n        FOREVER_DEADLINE,\n    ).transact({\n        "from": user_1\n    })\n\n    # Check the user_1 received ~0.284 ethers\n    assert weth.functions.balanceOf(user_1).call() / 1e18 == pytest.approx(0.28488156127668085)\n```\n\n[See the full example](https://github.com/tradingstrategy-ai/web3-ethereum-defi/blob/master/tests/test_uniswap_v2_pair.py).\n\n## Uniswap v2 price estimation example\n\n```python\n# Create the trading pair and add initial liquidity\ndeploy_trading_pair(\n    web3,\n    deployer,\n    uniswap_v2,\n    weth,\n    usdc,\n    1_000 * 10**18,  # 1000 ETH liquidity\n    1_700_000 * 10**18,  # 1.7M USDC liquidity\n)\n\n# Estimate the price of buying 1 ETH\nusdc_per_eth = estimate_buy_price_decimals(\n    uniswap_v2,\n    weth.address,\n    usdc.address,\n    Decimal(1.0),\n)\nassert usdc_per_eth == pytest.approx(Decimal(1706.82216820632059904))\n```\n\n[See full example](https://github.com/tradingstrategy-ai/web3-ethereum-defi/blob/34a9e1b948a4ef5a620ee520b568c0fd27c75457/tests/test_uniswap_v2_pair.py#L243).\n\n## How to use the library in your Python project\n\nAdd `web3-ethereum-defi` as a development dependency:\n\nUsing [Poetry](https://python-poetry.org/):\n\n```shell\npoetry add -D web3-ethereum-defi\n```\n\n# Development and contributing\n\n[Read development instructions](https://web3-ethereum-defi.readthedocs.io/development.html).\n\n# Version history\n\n- [Read changelog](https://github.com/tradingstrategy-ai/web3-ethereum-defi/blob/master/CHANGELOG.md).\n- [See releases](https://pypi.org/project/web3-ethereum-defi/#history).\n\n# Social media\n\n- [Join Discord for any questions](https://tradingstrategy.ai/community).\n- [Message us on Twitter](https://twitter.com/TradingProtocol)\n\n# Notes\n\nCurrently there is no [Brownie](https://eth-brownie.readthedocs.io/) support.\nTo support Brownie, one would need to figure out how to import an existing Hardhat\nbased project (Sushiswap) to Brownie project format.\n\n# History\n\n[Originally created for Trading Strategy](https://tradingstrategy.ai). \n[Originally the package was known as eth-hentai](https://raw.githubusercontent.com/tradingstrategy-ai/web3-ethereum-defi/master/docs/source/_static/hentai_teacher_mikisugi_by_ilmaris_d6tjrn8-fullview.jpg).\n\n# License \n\nMIT\n',
     'author': 'Mikko Ohtamaa',
     'author_email': 'mikko@tradingstrategy.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://tradingstrategy.ai',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `web3-ethereum-defi-0.8/PKG-INFO` & `web3-ethereum-defi-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: web3-ethereum-defi
-Version: 0.8
-Summary: Web3 Ethereum DeFi toolkit for smart contracts, Ethereum JSON-RPC utilities, Uniswap, PancakeSwap, wallets and automated test suites.
+Version: 0.9
+Summary: Web3-Ethereum-DeFi is a library for smart contracts, DeFi trading (Uniswap, PancakeSwap), Ethereum JSON-RPC, EVM transactions and automated test suites.
 Home-page: https://tradingstrategy.ai
 License: MIT
 Keywords: ethereum,cryptocurrency,uniswap,erc-20,pancakeswap,sushiswap,polygon,web3,blockchain
 Author: Mikko Ohtamaa
 Author-email: mikko@tradingstrategy.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=4.4.0,<5.0.0); extra == "docs"
+Requires-Dist: eth-bloom (>=1.0.4,<2.0.0)
+Requires-Dist: futureproof (>=0.3.1,<0.4.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: sphinx-autodoc-typehints[docs] (>=1.16.0,<2.0.0); extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0); extra == "docs"
 Requires-Dist: sphinx-sitemap (>=2.2.0,<3.0.0); extra == "docs"
+Requires-Dist: ujson (>=5.2.0,<6.0.0)
 Requires-Dist: web3[tester] (>=5.28.0,<6.0.0)
 Project-URL: Repository, https://github.com/tradingstrategy-ai/web3-ethereum-defi
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/web3-ethereum-defi.svg)](https://badge.fury.io/py/web3-ethereum-defi)
 
 [![Automated test suite](https://github.com/tradingstrategy-ai/web3-ethereum-defi/actions/workflows/test.yml/badge.svg)](https://github.com/tradingstrategy-ai/web3-ethereum-defi/actions/workflows/test.yml)
@@ -42,15 +45,15 @@
    * [Uniswap v2 trade example](#uniswap-v2-trade-example)
    * [Uniswap v2 price estimation example](#uniswap-v2-price-estimation-example)
    * [How to use the library in your Python project](#how-to-use-the-library-in-your-python-project)
 * [Development](#development)
    * [Build requirements](#build-requirements)
    * [Make](#make)
 * [Version history](#version-history)
-* [Discord](#discord)
+* [Social media](#social-media)
 * [Notes](#notes)
 * [History](#history)
 * [License](#license)
 
 ![Pepe chooses Web3 Ethereum DeFi and Python](https://raw.githubusercontent.com/tradingstrategy-ai/web3-ethereum-defi/master/docs/source/_static/pepe.jpg)
 
 **Pepe chooses web3-ethereum-defi and Python**.
@@ -275,17 +278,18 @@
 [Read development instructions](https://web3-ethereum-defi.readthedocs.io/development.html).
 
 # Version history
 
 - [Read changelog](https://github.com/tradingstrategy-ai/web3-ethereum-defi/blob/master/CHANGELOG.md).
 - [See releases](https://pypi.org/project/web3-ethereum-defi/#history).
 
-# Discord
+# Social media
 
-[Join Discord for any questions](https://tradingstrategy.ai/community).
+- [Join Discord for any questions](https://tradingstrategy.ai/community).
+- [Message us on Twitter](https://twitter.com/TradingProtocol)
 
 # Notes
 
 Currently there is no [Brownie](https://eth-brownie.readthedocs.io/) support.
 To support Brownie, one would need to figure out how to import an existing Hardhat
 based project (Sushiswap) to Brownie project format.
```

