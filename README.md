JamJam16R

아 이름 잘못정했다 16라운드니까 **잼잼이16R**로 변경해야징

데이터 압축
---------

BWT(Burrows-Wheeler Transform), MTF(Move-To-Front) 알고리즘은 사용

BWT
---- 

$$ 
S = "BANANA" 
$$ 

SortedPermutations
------------------

$$
\text{SortedPermutations}(S) = \begin{bmatrix}
ANABAN \\
ANANAB \\
BANANA \\
NABANA \\
NANABA \\
ABANAN \\
\end{bmatrix}
$$

$$
\text{BWT}(S) = \text{LastColumn}(\text{SortedPermutations}(S))
$$

$$
\text{BWT}(S) = "ANNBAA"
$$


MTF
---

$$
\text{MTF}(L) = E
$$


$$
L = BWT결과값
$$


$$
E = MTF인코딩된값
$$


Symmetric key encryption
------------------------

$$
K = 대칭키
$$

$$
IV = 초기벡터
$$

$$
D = 데이터
$$

$$
C = \text{QESAC-Encrypt}(K, IV, D)
$$

$$
D' = \text{QESAC-Decrypt}(K, IV, C)
$$

$$
D' = D
$$



Asymmetric key encryption
-------------------------

$$
K = 대칭키
$$


$$
e = 공개키
$$


$$
n = 모듈러스
$$


$$
C_K = K^e \mod n = 암호화된대칭키
$$

$$
A \cdot s + e \equiv b \pmod{q}
$$
