
# git 명령어

## 전역 설정 정보 조회


> git config - -global - -list

## 전역 설정 정보 삭제시키기


>1. git config --global --unset-all user.email


>2. git config --global --unset-all user.name

## 새로운 저장소 초기화하기

> git init

## 저장소 복제하기


> git clone <저장소 url>

## 새로운 원격 저장소 추가하기


> git remote add <원격 저장소> <저장소 url>

## 새로운 파일 git에 등록시키기(staging)


> git add <파일>

## 현재까지 작업한 내용 저장하기


> git commit -m “<메시지>”

## 원격 저장소에서 합치지 않고 지역 브랜치로 변경 사항 가져오기


> git fetch <원격 저장소>

## 원격 저장소에서 변경 사항을 가져와 현재 브랜치에 합치기


> git pull <원격 저장소>

## 새로운 로컬 브랜치를 원격 저장소에 푸싱하기


> git push <원격 저장소> <지역 브랜치>



# markdown 문법


## 제목(Headers)
 - 글씨 크기를 변환한다. ` # `의 갯수가 늘어날수록 글씨가 작아진다.

>입력
```
 # 가장 큰 제목 (H1)
 ## 두 번째 수준 제목 (H2)
 ### 세 번째 수준 제목 (H3)
 #### 네 번째 수준 제목 (H4)
 ##### 다섯 번째 수준 제목 (H5)
 ###### 여섯 번째 수준 제목 (H6)
```

>출력
>> # 가장 큰 제목 (H1)
>> ## 두 번째 수준 제목 (H2)
>> ### 세 번째 수준 제목 (H3)
>> #### 네 번째 수준 제목 (H4)
>> ##### 다섯 번째 수준 제목 (H5)
>> ###### 여섯 번째 수준 제목 (H6)


## 인용(Blockquotes)
 - 인용된 글을 표시한다. 한줄에 써도 되고 줄마다 인용해도 된다. ` > `를 사용한다.
>입력
```
 인용되지 않는 글입니다.
 >인용되는 글입니다. 인용되는 글입니다. 인용되는 글입니다. 인용되는 글입니다. 인용되는 글입니다. 인용되
 는 글입니다. 인용되는 글입니다. 인용되는 글입니다. 인용되는 글입니다.
 >인용되는 글입니다.
 >인용되는 글입니다.
 인용수준을 변경할 때 빈 줄 하나를 넣는다.
 인용되지 않는 글입니다.
 ```
 
>출력
>> 인용되지 않는 글입니다.
>> >인용되는 글입니다. 인용되는 글입니다. 인용되는 글입니다. 인용되는 글입니다. 인용되는 글입니다. 인용되는 글입니다. 인용되는 글입니다. 인용되는 글입니다. 인용되는 글입니다.\
>> >인용되는 글입니다.\
>> >인용되는 글입니다.
>>
>> 인용되지 않는 글입니다.
 
 - ` >> `를 사용하여 인용된 글 안에서 또 다시 글을 인용하는 것도 가능하다.
 
>입력
```
 인용되지 않는 글입니다.
 >인용되는 글입니다.
 >> 또 다시 인용되는 글입니다.
 >> 또 다시 인용되는 글입니다.
 >인용수준을 변경할 때 빈 줄 하나를 넣는다.
 >인용되는 글입니다.
 인용되지 않는 글입니다.
 ```
 
 >출력
>> 인용되지 않는 글입니다.
>> >인용되는 글입니다.
>> >> 또 다시 인용되는 글입니다.\
>> >> 또 다시 인용되는 글입니다.
>> 
>> >인용되는 글입니다.
>>
>> 인용되지 않는 글입니다.
 
 
 ## 코드블럭(code Blocks)
 -코드를 감싸서 코드를 그대로 보여주고 싶을 때 사용한다. 짧은 코드는` ' `를 사용한다.
 
 >입력
 ```
 `<table><tr><td></td></tr></table>`
 ```

>출력
>> `<table><tr><td></td></tr></table>`

-줄이 한 줄이 아닐 때는 시작 줄과 끝 줄에 ` ` `기호나 ` ~ `기호를 세개 쓴다.

>입력
``` ```
void f()
    printf(%s,“이것은 c 코드 입니다”);
}
``` ```

>출력

```
void f()
    printf(%s,“이것은 c 코드 입니다”);
}
```


## 강조 Emphasis
-기울여 쓰기(italic)는 ` * ` 또는 ` _ `로 감싸고 굵게 쓰기(bold)는 ` ** ` 또는 ` __ `로 감싼다.
