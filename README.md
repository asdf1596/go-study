###go-study

##변수

기본적으로는 var을 사용해서 선언한다

var (변수이름) (변수형)의 형태로 선언한다.

예시: var int1 int = 1 or int1 := 1

이렇게 쓰여있지만 전역변수가 아니면

(변수명) := (값) 으로 쓴다.

형은 알아서 go가 추정을 해준다.

#정수

기본적으로는 int를 사용하지만 int도 uint,uint8,uint64,int64등 다양하다

다양한 이유는 쓸데없는 메모리의 사용을 줄이기 위해서 범위를 지정하기 때문이다.

#실수형

float32, float64가 있으면 2개가 있는 이유는 정수와 같다.

#문자형

string만이 존재한다.

#포인터형(변수 주소)

uintptr, uint와 크기가 같다

#그 외

bool:참거짓 표현용(8비트)

byte:8비트 자료형

rune:유니코드 저장용, int32와 크기가 같다

주의점: go에서 ":="하고 "="는 다르다 앞은 선언과 동시에 대입이고 뒤는 그냥 대입이다.

##연산자

대부분이 c와 동일하기에 큰 설명이 필요없다.

사용 가능한 연산자들

a = 1+1,b = 1-1,c = 1\*1,d = 1/1

a+=1,b-=1,c\*=1,d/=1,e%=1

a = b & c(and),a = b | c(or),a = b ^ c(xor),a = b &^ c(and not)

a &= b,a |= b,a ^= b,a &^= b

a = b << c,a = b >> c,a = ^b(비트 반전)

a = +b(값X+),a = -b(값X-)

==,!=,<=,>=,<,>

&&,||,!

a = &b(b의 메모리 주소값)

\*a = 1(메모리의 값이 a인 값을 바꿈)

++,--
