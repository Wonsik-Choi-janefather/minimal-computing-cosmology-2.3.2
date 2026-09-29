# 14장 선언을 유한 실행계로 옮기기

WRRA는 말의 체계에 머물지 않기 위해 양의 스펙트럼, 자기수반 Hamiltonian, visible port, 복원 gap과 엔트로피 장부가 동시에 존재하는 유한 benchmark를 구성했다.

H\_N = H\_Jacobi ⊗ H\_loc ⊗ H\_syn (14.1)

출발점은 threshold s₀ 위의 양의 generalized-Laguerre spectral density다. α>−1이면 정규화가 가능하며, 직교다항식의 삼항점화식은 실수 대칭 Jacobi 행렬을 결정한다.

ρ(s)=((s−s₀)^α e<sup>{−(s−s₀)/Λ²})/(Γ(α+1)Λ</sup>{2α+2}) Θ(s−s₀) (14.2)

(J\_N)nn=s₀+Λ²(2n+α+1), (J\_N)n,n+1=Λ²√((n+1)(n+1+α)) (14.3)

첫 기저벡터 e₀를 visible port로 선택하면 고유값의 가중치는 첫 성분의 제곱이 되어 자동으로 비음수이고 합이 1이다. 하나의 collective coordinate가 N개의 숨은 spectral node를 읽는다. Euclidean 응답과 실시간 진폭도 같은 node와 weight에서 나온다.

G\_E(Q²)=∫ρ(s)/(Q²+s)ds = Σ\_j w\_j/(Q²+s\_j) (14.4)

A\_N(t)=Σ\_j w\_j e^{−is\_jt} (14.5)

N=2,4,8,16,32에서 지정된 Euclidean 창의 최대 상대오차는 4.089×10⁻²에서 1.763×10⁻⁹까지 감소했다. 반면 유한 스펙트럼은 장시간 recurrence를 남긴다. 이 차이는 “유한계가 연속체를 정확히 흉내 내는 시간창”과 “영구적인 비가역성”을 분리한다.

복원 sector에는 amplitude-damping형 Lindblad 연산자를 두어 syndrome-transverse gap을 정확히 계산했다.

L\_rec(ρ)=κ\[σ₋ρσ₊−½{σ₊σ₋,ρ}], Δ\_corr=κ/2 (14.6)

ΔS\_rec=−p ln p−(1−p)ln(1−p), Q\_min=k\_BTΔS\_rec (14.7)

이 benchmark의 가치는 우주 전체를 복제했다는 데 있지 않다. WRRA가 요구한 양성·자기수반성·공통 visible port·유한창 수렴·복원·metric 보존·열역학 장부가 한 유한 구조에서 서로 모순 없이 공존할 수 있음을 보였다는 데 있다.
