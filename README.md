
## PG Analytics - 결제데이터 분석서비스
* 기존 PG 사를 이용 중이신 사업자도 별도의 계약없이 부트페이를 통해 결제 연동과 통계를 무료로 이용하실 수 있습니다.
* 한줄의 소스코드로 인사이트를 얻어 매출을 극대화하세요.



## 결제 검증 및 취소 - 서버사이드용
* 보안상의 이유로 결제검증과 취소는 서버사이드에서 이루어집니다.
* 부트페이 서버와 통신시 Rest용 Application Id, Private Key 값을 보내주셔야 하며, 보내실 서버의 IP는 미리 등록하셔야 합니다.

## requirements.txt에 아래 내용 추가 
```
//requirements.txt 파일에 아래 내용을 추가
requests==2.18.3
```

## 추가된 requirements.txt 를 통해 requests 설치 
```
pip install -r requirements.txt
```

## 샘플 코드
```python 
from lib.BootpayApi import BootpayApi

api = BootpayApi("application_id_value_1234", '593f8febe13f332431a8ddaw')
print api.verify('593f8febe13f332431a8ddae').text
```

### 더 자세한 정보는 [Docs](https://docs.bootpay.co.kr/api/validate?languageCurrentIndex=3)를 참조해주세요. 
