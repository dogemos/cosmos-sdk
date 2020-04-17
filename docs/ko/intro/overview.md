<!--
order: 1
-->

# High-level Overview

## 코스모스 SDK는 무엇인가?

The [Cosmos-SDK](https://github.com/cosmos/cosmos-sdk) is an open-source framework for building multi-asset public Proof-of-Stake (PoS) <df value="blockchain">blockchains</df>, like the Cosmos Hub, as well as permissioned Proof-Of-Authority (PoA) blockchains. 코스모스 SDK를 사용하여 만들어진 블록체인은 통상 **애플리케이션 특화 블록체인(application-specific blockchain) 이라 불립니다.**

코스모스 SDK의 목적은 개발자가 간편하게 처음부터 다른 블록체인과 상호환이 가능한 블록체인을 만들 수 있게 하는 것이 목적입니다. 코스모스 SDK는 npm과 같은 프레임워크로 자리잡으며 [텐더민트](https://github.com/tendermint/tendermint) 상의 안전한 블록체인 애플리케이션을 만들 수 있게 자리잡는 것이 목표입니다. SDK-based blockchains are built out of composable [modules](../building-modules/intro.md), most of which are open source and readily available for any developers to use. 누구나 코스모스 SDK 모듈을 만들 수 있으며, 단순히 블록체인 애플리케이션에 모듈을 불러와 이미 개발된 모듈을 간편하게 사용할 수 있습니다. 또한, 코스모스 SDK는 능력성 기반(capabilities-based) 시스템으로 모듈 간 인터랙션의 보안성을 더욱 직관적으로 설계할 수 있습니다. For a deeper look at capabilities, jump to [this section](../core/ocap.md).

## 애플리케이션 특화 블록체인은 무엇인가?

최근 블록체인 업계의 개발 패러다임 중 하나는 이더리움과 같은 버추얼 머신(virtual-machine) 기반 블록체인입니다. 이런 시스템에서는 기존 블록체인 상위에 스마트 컨트랙트 기반의 탈중앙화 애플리케이션을 만드는 형태로 개발됩니다. While smart contracts can be very good for some use cases like single-use applications (e.g. ICOs), they often fall short for building complex decentralised platforms. 스마트 컨트랙트는 유연성, 존엄성 그리고 성능 측면에서 한계가 존재합니다.

애플리케이션 특화 블록체인은 기존 버추얼 머신 기반 블록체인과는 획기적으로 다른 개발 패러다임을 제공합니다. 애플리케이션 특화 블록체인은 하나의 애플리케이션을 구동하기 위해 특화되며, 개발자는 애플리케이션이 최적한 환경에서 구동될 수 있는 디자인 결정을 내릴 수 있습니다. 또한 애플리케이션 특화 블록체인은 애플리케이션 존엄성, 보안 그리고 성능 측면에서 장점을 가집니다.

Learn more about [application-specific blockchains](./why-app-specific.md).

## 왜 코스모스 SDK인가?

코스모스 SDK는 고유 애플리케이션 특화 블록체인을 만들기 위한 가장 우수한 프레임워크입니다. 다음은 코스모스 SDK가 탈중앙화 애플리케이션을 개발하는데 제공하는 장점들입니다:

- 코스모스 SDK가 기본적으로 제공하는 합의 엔진은 [텐더민트 코어](https://github.com/tendermint/tendermint)입니다. 텐더민트는 가장 (유일하게) 오랜 기간 증명된 BFT 기반 컨센서스 엔진입니다. 텐더민트 코어는 업계 내의 수 많은 환경에서 지분증명 시스템을 개발하는데 사용되고 있습니다.
- The SDK is open source and designed to make it easy to build blockchains out of composable [modules](../../x/). As the ecosystem of open source SDK modules grows, it will become increasingly easier to build complex decentralised platforms with it.
- 코스모스 SDK는 능력성 기반(capabilities-based) 보안 아키텍쳐를 기반으로 설계되었습니다. 이런 디자인 결정은 수년간 블록체인 스테이트 머신(state machine)에 대한 고민을 기반으로 설계되었으며, 더욱 안전한 블록체인을 개발할 수 있는 환경을 제공합니다.
- 가장 중요한 것은 바로 코스모스 SDK가 실제 작동하고 있는 다수의 애플리케이션 특화 블록체인을 개발하는데 사용되고 있다는 점입니다. Among others, we can cite [Cosmos Hub](https://hub.cosmos.network), [IRIS Hub](https://irisnet.org), [Binance Chain](https://docs.binance.org/), [Terra](https://terra.money/) or [Kava](https://www.kava.io/). [Many more](https://cosmos.network/ecosystem) are building on the Cosmos SDK.

## 코스모스 SDK 입문하기

- Learn more about the [architecture of an SDK application](./sdk-app-architecture.md)
- 애플리케이션 특화 블록체인을 처음부터 개발하는 방법을 [코스모스 SDK 투토리얼](https://cosmos.network/docs/tutorial)을 통해 배워보세요

## Next {hide}

Learn about [application-specific blockchains](./why-app-specific.md) {hide}
