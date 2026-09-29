# 제2부. 미시구조 보강

## 4장. 중력의 미시재료

MCC 2.0에서 중력의 핵심은 owner이다. 중력은 특정 gauge charge가 아니라 구현된 전체 물리자유도의 stress-energy를 읽는다. string theory를 가져와도 이 ownership은 바뀌지 않는다.

**Equation (4.1)**

O\_G(X) = T\_μν\[X], O\_a(X) = J\_a\[X]

string theory에서는 closed-string spectrum에 massless spin-2 excitation이 존재하고, low-energy limit에서 Einstein-Hilbert형 gravity와 higher-curvature correction이 나타난다. 이 점은 MCC에서 아직 약했던 ’왜 quantum microscopic sector와 gravity가 같은 내부 이론 안에서 일관될 수 있는가’를 보강한다.

**Equation (4.2)**

S\_4^grav = ∫ d⁴x √−g \[ (M\_P²/2)R + α’ c₁R² + α’² c₂R³ + … ]

MCC의 역할은 higher-curvature term을 모두 fundamental Reality에 항상 활성화하는 것이 아니다. 저곡률에서 Einstein term만으로 viability가 유지되면 최소 실행은 leading sector를 사용하고, 고곡률에서 필요한 correction만 활성화되는 effective redundancy로 해석한다.

**Statement**

소유권 보존 string graviton은 ’중력=네 번째 gauge current’로 바꾸지 않는다. closed-string origin과 관계없이 4D Reality에서 중력 owner는 여전히 total Tμν이며, 세 gauge force는 representation current를 선택적으로 읽는다.

## 5장. 게이지·anomaly·BRST 폐쇄

MCC 2.0의 중요한 OPEN 중 하나는 공통 carrier와 gauge matter를 전체 anomaly-free microscopic realization으로 닫는 일이다. heterotic string은 이 부분에서 직접적인 수리 재료를 제공한다. 10D consistency와 Green–Schwarz mechanism은 gauge/gravitational anomaly를 상쇄하는 매우 강한 구조를 갖는다.

**Equation (5.1)**

H = dB − (α’/4)(ω\_3Y − ω\_3L)

**Equation (5.2)**

dH = (α’/4)\[ tr(R∧R) − Tr(F∧F) ]

부호와 trace normalization은 convention에 따라 달라질 수 있지만 구조적 핵심은 gauge bundle과 tangent bundle의 topology가 독립 장부가 아니라 B-field의 consistency condition으로 묶인다는 점이다. MCC 관점에서는 이것이 ‘추가 자유도가 스스로 비용을 지불하는’ 좋은 사례다. B-field는 장식이 아니라 anomaly closure를 수행한다.

따라서 기존 WRRA의 conditional BRST closure는 다음처럼 역할을 나눌 수 있다. 10D microscopic anomaly/BRST consistency는 IMPORTED STRING CONSTRAINT, 4D renderer path independence와 protected-observable recovery는 WRRA CONSTRAINT이다. 둘은 같은 문제가 아니다.

## 6장. 공통운반자의 미시 구현

본 보강의 핵심 장이다. WRRA의 abstract common carrier를 string compactification의 공통 bundle-covariant operator와 연결한다. compact space K6와 gauge bundle V 위의 10D fermionic kinetic operator를 다음처럼 둔다.

**Equation (6.1)**

𝒟\_(10,V) = Γ^M(∇\_M + A\_M)

product/warped compactification에서 fermionic field를 내부 eigenmode로 전개한다.

**Equation (6.2)**

Ψ(x,y) = Σ\_n ψ\_n(x) ⊗ ξ\_n(y), 𝒟\_(K,V) ξ\_n = λ\_n ξ\_n

저에너지 chiral matter는 적절한 zero mode 또는 light mode에서 나온다. 중요한 점은 서로 다른 4D channel이 서로 다른 독립 운반자를 요구하는 것이 아니라, 같은 10D covariant operator와 같은 compactification geometry/bundle에서 내려온다는 것이다.

**Equation (6.3)**

D\_C^(4) ≔ P\_15 · Red\_(K6)\[𝒟\_(10,V)] · P\_15

식 (6.3)은 표준 string theory의 정리라기보다 MCC가 제안하는 microscopic identification이다. P15는 한 세대의 15개 카이럴 Standard Model channel을 선택하는 projector이고, Red\_K6는 compactification/reduction map이다. 이 identification이 성립한다면 공통운반자는 ’추상적으로 하나’에서 ’미시적으로 어떤 operator인가’까지 한 단계 내려간다.

**Statement**

공통운반자의 보존 String은 carrier의 재료이지 carrier를 삭제하는 이름이 아니다. 10D common operator → 여러 internal zero modes → 15개 4D channel이라는 계보를 가져야만 MCC의 공통운반자 조건을 만족한다.

## 7장. 카이럴 15채널과 세대

4D chirality는 compactification의 가장 중요한 string 자원 중 하나다. bundle-covariant internal Dirac operator의 index는 left/right zero mode의 순차이를 topology와 연결한다.

**Equation (7.1)**

N\_L − N\_R = index(𝒟\_(K,V))

따라서 ’왜 chiral matter가 가능한가’는 MCC 단독보다 훨씬 강하게 보강된다. 다만 index가 자동으로 3을 준다고 주장해서는 안 된다. 세 세대를 얻으려면 geometry/bundle/topological data가 net chirality 3을 주는 compactification을 선택해야 한다.

**Equation (7.2)**

index(𝒟\_(K,V)) = 3 (target condition, not automatic identity)

MCC가 새로 하는 일은 많은 topology 가운데 ’3을 만들 수 있다’는 것만으로 끝내지 않고, 관측계약을 만족하는 후보 중 전체 computation/structure cost가 가장 작은 것을 선택하는 것이다.

한 세대 15채널은 Standard Model representation에 따라 분해되지만 그 전달골격은 식 (6.3)의 common carrier에서 공유한다. 세대 수는 common carrier를 세 번 복제하는 것으로 정의할 필요가 없다. 동일한 carrier operator의 서로 다른 내부 zero-mode family가 세대를 구성할 수 있다.

## 8장. 표현형으로서의 물질

string phenomenology에서 4D 입자 spectrum은 compactification geometry, brane/bundle data, symmetry breaking과 moduli에 민감하다. MCC는 이것을 약점으로만 보지 않는다. ’물질은 숫자 목록이 아니라 실행 표현형’이라는 기존 주장을 미시적으로 설명할 재료가 된다.

**Equation (8.1)**

Φ\_string → {ξ\_i(y), r\_i, q\_i} → 4D field ψ\_i(x) → SSB/Yukawa → RG/dressing → pole/record

물리모형 1.0의 compact witness에서는 n/R이 이산 질량 전구체와 전하를 함께 만든다. 선택적 string compactification은 이 구조의 미시 구현 후보를 제공할 수 있고, Reality의 질량은 Higgs/Yukawa·moduli dependence·self-energy·QCD dressing을 거쳐 안정된 pole로 나타난다. 따라서 ‘모든 질량은 string vibration number 하나’로 단순화하지 않으며, string이 앞선 질량 양자화 결과를 대체한다고도 쓰지 않는다.

**Equation (8.2)**

m\_f(μ) = y\_f(μ)v(μ)/√2, det S\_f^(−1)(p)|\_(p²=m\_pole²) = 0

string-derived Yukawa coupling은 내부 wavefunction overlap 또는 geometry에 의해 결정될 수 있다. schematic하게 다음과 같이 쓸 수 있다.

**Equation (8.3)**

Y\_ijk ∼ ∫\_(K6) 𝒲\_i(y) 𝒲\_j(y) 𝒲\_k(y) · measure(K6)

그러나 최종 물리 입자는 이 coupling 자체가 아니다. WRRA의 phenotype map이 mass, charge, spin, location, history와 record를 하나의 object에 공동귀속시킨다.

**Equation (8.4)**

Object X ⇔ co-owned{m,q,s,x} on (A\_local, history, pole, record)

**Statement**

표현형 불변성 끈이론을 가져온 뒤에도 ’입자는 string vibration이다’로 끝내지 않는다. string mode는 genotype-like microscopic material이고, 관측 입자는 4D execution과 renderer를 거친 phenotype이다.
