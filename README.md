# blockchain
DApp, DeFi

# Flash Loan을 이용한 차익거래 프로그래밍
담보없이 Flash Loan 받아 차익거래로 수익을 창출

## Background
- **Flash Loan 이란 ?**
 전통적인 대출의 경우 대부업자는 일반적으로 돈을 상환받기 위해 어떤 형태의 담보나 담보를 요구합니다. 대출 계약은 일반적으로 승인되는 데 시간이 걸리며 차용인은 정해진 기간 동안 이자  와 함께 대출금을 상환합니다.
 반면에 플래시론은 순식간에 발생합니다. 자금은 한 거래 공간에서 빌리고 반환됩니다. 이것은 조건을 설정하고 차용인을 대신하여 수수료를 받는 즉시 거래를 수행하는 스마트 계약을 통해 가능합니다. 이 수수료를 "가스 수수료"라고 합니다.
 차용인이 대출금을 상환하지 않거나 거래가 이익을 내지 못하면 스마트 계약의 조건이 충족되지 않습니다. 그런 다음 거래가 취소되고 자금이 대출 기관에 반환됩니다. 스마트 계약으로 인해 대 출자와 대출자 모두에게 최소한의 위험이 있습니다.
 즉 담보없이 대출을 실행하고 한 계약안에서 상환이 일어납니다. 
 최소한의 위험으로 대부업자 대출자에게 노출이되면서 무담보 대출을 사용할 수 있게 됩니다.
 트랜젝션 하나에 대출과 상환이 포함되어 있어 가능한 부분이 되었습니다. 

- **차익거래란** ?
 전통적인 금융 세계에서 차익 거래는 투자자가 서로 다른 시장에서 동시에 자산을 사고 팔아 가격 차이를 이용하고 이익을 창출하는 투자 전략입니다. 일반적으로 가격 차이는 작지만 큰 볼륨을  곱하면 수익이 인상적일 수 있습니다. 재정 거래는 일반적으로 전통적인 금융 시장에서 헤지 펀드 및 기타 정교한 투자자가 활용합니다.
 DeFi 세계에서 거래자는 차익 거래 전략을 사용하여 자산에 대해 서로 다른 가격을 제공하는 플랫폼 간 거래를 통해 이익을 얻을 수 있습니다. 거래자는 금전적 이익을 얻기 위해 암호화폐 자산을 다른 가격에 사고 팔아 시장의 비효율성을 이용할 수 있습니다.
 플래시 론을 사용함으로써 트레이더는 두 개의 분산형 거래소에서 차익 거래를 실행하기 위해 많은 돈을 빌릴 수 있습니다. 즉시 대출과 차익 거래 전략을 결합함으로써 트레이더는 수익 잠재력을 높일 수 있습니다.

- **가격 슬리피지**
가격 슬리피 지는 거래의 예상 가격과 거래가 실행되는 가격의 차이를 말합니다. 일반적으로 단기간에 시장 변동성이 크거나 현재 거래량이 기존 매수/매도 스프레드를 초과할 때 발생합니다.

- **탈중앙화 거래소(DEX)** 
중개자 없이 온라인에서 안전하게 P2P 암호화폐 교환이 이루어질 수 있도록 하는 일종의 암호화폐 거래소입니다.

- **DEX 애그리게이터** 
다양한 DEX에서 유동성을 공급하므로 사용자에게 단일 DEX보다 더 나은 토큰 스왑 비율을 제공합니다.
유동성 풀 은 DEX에 유동성을 제공하기 위해 스마트 계약에 잠긴 자금 모음입니다. 유동성 풀의 장점은 구매자와 판매자 간의 주문 일치가 필요하지 않고 대신 슬리피지가 적은 사전 자금 조달 유동성 풀을 활용한다는 것입니다.

- **Orderbook**
Orderbook 는 매수 및 매도 주문 모음으로 구성됩니다. 입찰가와 요청가가 동일한 경우에만 주문이 일치되고 실행됩니다.
중앙화된 거래소인 업비트, 빗썸 에서 이용되는 방법

- **AMM ( Automated Market Maker)** 
주문서 대신 유동성 풀을 사용하고 수학적 공식을 사용하여 자산 가격을 책정합니다. 자산은 풀의 최신 가격에 대해 자동으로 교환될 수 있으므로 기존 주문서보다 더 효율적입니다.

- **Wrapped ETH(WETH)** 
이더리움의 ERC20 거래 가능 버전입니다. WETH는 ETH보다 스마트 계약 내에서 거래하기가 더 쉽습니다. 또한 사용자는 WETH를 거래소에 보낸 후 WETH에 대한 액세스 권한을 취소할 수 있습니다. 이는 ETH로는 불가능합니다. Flash Loan 거래시에 ETH가 아닌 WETH를 이용하여 거래에 사용


## Summary
 - **중앙 집중식 거래 vs DeFi 차익 거래의 차이**
    - **DeFI**
    미리 결정된 매개 변수에 따라 스마트 계약이 자동으로 실행되므로 지급 불능 위험이 최소화됩니다. 예상대로 실행될 수 없는 경우 거래가 취소됩니다.
    트레이더는 플래시 론으로 빌린 자금을 사용하여 차익 거래를 수행할 수 있습니다.
    - **중앙 집중식 거래**
     트레이더는 동시에 거래를 실행할 수 없기 때문에 거래가 지연되면 가격 하락을 겪을 수 있습니다.
     트레이더는 자금을 소유하거나 은행에서 차입해야 합니다.

- AMM을 사용하는 DEX 간의 차익 거래
  - **인기 있는 플랫폼**
    - [Uniswap](https://uniswap.org/), [Balancer](https://balancer.fi/), [1inch](https://app.1inch.io/), [Sushi Swap](https://app.sushi.com/), [Kyber Network](https://kyber.network/),  and [Curve Finance](https://curve.fi/#/ethereum/swap).

  - **시나리오** 
    - DEX 풀간 자산 교환 가격차이가 발생 하는 경우
  - **실행**
    - 한 풀에서 자산 A에서 자산 B로 Swap하고 다른 풀에서 다시 Swap하여 두 풀 사이의 가격 스프레드에서 이익을 얻는다
   
- 클래식 오더북을 사용하는 DEX 간 차익거래
 - 인기 있는 플랫폼
  0x 프로토콜 로 구동되는 Radar Relay


## 플래시 론의 실행 단계 

1. 대출자는 플래시 대출 스마트 계약을 실행합니다.
2. 플래시론 계약은 유동성 풀에서 대출 금액을 요청합니다. 
3. 그런 다음 계약은 정의된 작업(예: 거래소에서 거래)을 실행하기 위해 대출 자금을 사용합니다. 
4. 운영 완료 후 차입금은 유동성 풀로 반환 
5. 트랜잭션이 블록체인에 커밋됩니다. 

스마트 계약을 통해 다음을 검증할 수 있습니다. 

플래시론에는 스마트 계약에서 작업을 수행하는 데 필요한 자금이 있습니다. 
트랜잭션이 새 블록에 추가되기 전에 작업이 완료됩니다. 
운영으로 인해 차용인의 자금 손실이 발생하지 않습니다. 
렌딩 풀은 프로토콜 사용에 대한 정확한 금액 + 거래 수수료를 돌려받습니다. 
차용인은 대출 기관이 수정된 대출 금액을 상환받는 한 자금으로 원하는 모든 것을 할 수 있습니다. 

- Flash Loan의 인기 사용 사례 
 - 거래 차익 거래 - 이익을 내기 위해 한 거래소에서 더 높은 가치를 가진 다른 거래소로 토큰을 가져갑니다.
 - 담보 스왑 - 담보 대출의 토큰을 기존 대출의 담보로 다른 토큰으로 교환
 - 자기 청산 - 토큰 스왑을 통한 담보 대출 상환 및 플래시 론 상환





## Direct Usage of Smart Contracts

![flash-loan-diagram](https://user-images.githubusercontent.com/117779419/208811327-4bceff38-f885-4d3b-b158-da4964602cc7.png)




## 코딩없이 플래시론 사용하기 furucombo web site 의 사용방법

```
wget  
```

1.Flash loan Aave\
2.Swap Token 1inch\
3.Swap Token Curve\
4.Repay Loan Aave

![frurucombo-flashloan](https://user-images.githubusercontent.com/117779419/206181242-17944c56-a1e3-4af0-89ae-9e3542bc725a.PNG)
