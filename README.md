# 마크다운 작성법

## 목차
[1. 헤더](#1-header-헤더)
[2. 강조](#1-emphasis-강조)
[3. 인용](#3-blockquotes-인용)
[4. 목록](#4-list-목록)
[5. 백슬래쉬 이스케이프](#5-backslash-escapes-백슬래쉬-이스케이프프)
[6. 이미지](#6-images-이미지)
[7. 링크](#7-link-링크)
[8. 코드 블럭](#8-fenced-code-blocks-코드-블럭)
[9. 체크 리스트](#9-task-list-체크-리스트)
[10. 수평선](#10-horizontal-rules-수평선)
[11. 테이블](#11-table-테이블)
[12. 줄바꿈](#12-line-breaks-줄바꿈)

## 1. Header 헤더
* `#`으로 시작
* 1개부터 6개까지
* H1 (`===`)
* H2 (`---`)
### 헤더 Syntax
    This is H1 Sentence
    ===
    This is H2 Sentence
    ---
    # This is H1 Sentence
    ## This is H2 Sentence
    ### This is H3 Sentence
    #### This is H4 Sentence
    ##### This is H5 Sentence
    ###### This is H6 Sentence
### 헤더 실행결과
# This is H1 Sentence <br>
## This is H2 Sentence <br>
### This is H3 Sentence <br>
#### This is H4 Sentence <br>
##### This is H5 Sentence <br>
###### This is H6 Sentence <br>
    
## 2. Emphasis 강조
* 기울이기(italic): `*`또는 `_`로 감싼 텍스트
* 굵게(bold): `**`또는 `__`로 감싼 텍스트
* 취소선: `~`로 감싼 텍스트
### 강조 Syntax
    *This text italic*
    _This text italic too_
    **This text bold**
    __This text bold too__
    ~~This text cancled~~
    **This text *italic* and bold**
### 강조 실행결과
This text italic* <br>
_This text italic too_ <br>
**This text bold** <br>
__This text bold too__ <br>
~~This text cancled~~ <br>
**This text *italic* and bold** <br>
## 3. Blockquotes 인용
* `>`로 시작하는 텍스트
* `>`는 3개까지 가능
### 인용 Syntax
    Use Blockquotes
    > This sentence uses first quotation
    >> This is second blockquote
    >>> This is third blockquote
### 인용 실행결과
Use Blockquotes
> This sentence uses first quotation
>> This is second blockquote
>>> This is third blockquote
## 4. List 목록
### 4.1 순서가 없는 목록
* `*`, `+`, `-`를 이용해서 순서가 없는 목록을 만든다
* 들여쓰기를 하면 모양이 바뀐다
### 4.2 순서가 있는 목록
* 숫자를 기입해서 순서가 있는 목록 사용
* 들여쓰기를 하면 모양이 바뀐다
### 목록 Syntax
    * itme 1
    * item 2
       * item 1-1
       * item 2-1
         * item 1-2
         * item 2-2
    1. item 1
    2. item 2
       1. item 1-1
       2. item 2-1
          1. item 1-2
          2. item 2-2
### 목록 실행결과
* itme 1
    * item 2
      * item 1-1
      * item 2-1
        * item 1-2
        * item 2-2
1. item 1
2. item 2
   1. item 1-1
   2. item 2-1
      1. item 1-2
      2. item 2-2
## 5. Backslash Escapes 백슬래쉬 이스케이프
* 특수문자를 표현할 때, 표시될 문자 앞에 `\`를 넣는다
* `감싸는 형태가 아니라` 문자의 앞, 뒤 모두 백슬래쉬 뒤에 특수문자가 온다
* \ backslash, \ backtick, * asterisk, _ underscore, {} curly braces, [] square brackets, () parentheses, # hash mark, + plus sign, - minus sign (hyphen), . dot, ! exclamation mark
### 백슬래쉬 이스케이프 Syntax
    \*literal asterisks\*
    \#hash mark\#
    \[squre brackets\]
### 백슬래쉬 이스케이프 실행결과
\*literal asterisks\* <br>
\#hash mark\# <br>
\[squre brackets\] <br>
## 6. Images 이미지
* 앞에 `!`가 붙는다
* 인라인 이미지: ![alt text](/image.jpg)
* 링크 이미지: ![alt text](image url)
* 이미지 사이즈 변경: `<img width="OOOpx" height="OOOpx"></img>`와 같이 표현
### 이미지 Syntax
    ![사진 설명](/image.png)
### 이미지 실행결과
![풍경사진](/image.jpg) <br>
##7. Link 링크
### 7.1 외부 링크
    인라인 링크: [링크](http:/.example.com "링크 제목") 
    ulr 링크: <example.com>, <example@example.com>; 꺽쇠 괄호 없어도 자동으로 링크를 사용
### 외부 링크 Syntax
    [Google](https://www.google.com "구글")
    [Naver](https://www.naver.com "네이버")
    구글 www.google.com; 꺽쇠X
    네이버 <www.naver.com>; 꺽쇠O
    E-mail <example@example.com>
### 외부링크 실행결과
[Google](https://www.google.com "구글") <br>
[Naver](https://www.naver.com "네이버") <br>
구글 www.google.com;  꺽쇠X <br>
네이버 <www.naver.com>;  꺽쇠O <br>
E-mail <example@example.com> <br>
### 7.2 내부 링크
    [보여지는 내용](#이동할 헤드(제목))
    괄호 안의 링크를 쓸 때는 띄어쓰기는 -로 연결, 영어는 모두 소문자로 작성
### 내부 링크 Syntax
[1. 헤더](#1-header-헤더) <br>
[2. 강조](#1-emphasis-강조) <br>
[3. 인용](#3-blockquotes-인용) <br>
### 내부 링크 실행결과
[1. 헤더](#1-header-헤더)
[2. 강조](#1-emphasis-강조)
[3. 인용](#3-blockquotes-인용)
## 8. Fenced Code Blocks 코드 블럭
* 간단한 인라인 코드는 텍스트 앞뒤로 `기호로 감싼다
* \`\`\` 혹은 ~~~ 코드
* 첫 줄과 마지막 줄에 (```) 또는 (~~~) 삽입
* 앞에 공백 네 칸 추가
* \`\`\`옆에 언어를 지정해주면 syntax color 적용
### 코드 블럭 Syntax
    ```
    This is code blocks
    ```

    ~~~
    This is code blocks
    ~~~

    ```python
    name = Tom
    print(f"Hello {name}!")
    ```
### 코드 블럭 실행결과
```
This is code blocks
```

~~~
This is code blocks
~~~

```python
name = Tom
print(f"Hello {name}!")
```
## 9. Task List 체크 리스트
* 줄 앞에 `- [x]`를 써서 완료된 리스트 표시
* 줄 앞에 `- [ ]`를 써서 미완료된 리스트 표시
* 체크 안에서 강조 외에 여러 기능 사용 가능
### 체크 리스트 Syntax
    - [x] this is a complete item
    - [ ] this is an incomplete item
    - [x] @mentions, #refs, [links](),
    **formatting**, and <del>tags</del>
    supported
    - [x] list syntax required (any
    unordered or ordered list
    supported)
### 체크 리스트 실행결과
- [x] this is a complete item
- [ ] this is an incomplete item
- [x] @mentions, #refs, [links](),
**formatting**, and <del>tags</del>
supported
- [x] list syntax required (any
unordered or ordered list
supported)
## 10. Horizontal Rules 수평선
* `-` 또는 `*` 또는 `_`을 3개 이상 작성
* 단, `-`을 사용할 경우 헤더로 인식할 수 있으니 이전 라인은 비워야 한다
### 수평선 Syntax
    * * *
    ***
    ******
    - - - 
    ----------
### 수평선 실행결과
* * *
***
******
- - - 
----------
## 11. Table 테이블
* 헤더와 셀을 구분할 때 3개 이상의 `-`기호가 필요
* 헤더 셀을 구분하면서 `:` 기호로 셀(열/칸) 안에 내용을 정렬
* 가장 좌측과 가장 우측에 있는 `|` 기호는 생략 가능
### 테이블 Syntax
테이블 생성

    헤더1|헤더2|헤더3|헤더4
    ---|---|---|---
    셀1|셀2|셀3|셀4
    셀5|셀6|셀7|셀8
    셀9|셀10|셀11|셀12
    
    테이블 정렬
    
    헤더1|헤더2|헤더3
    :---|:---:|---:
    Left|Center|Right
    1|2|3
    4|5|6
    7|8|9
### 테이블 실행결과
테이블 생성

헤더1|헤더2|헤더3|헤더4
---|---|---|---
셀1|셀2|셀3|셀4
셀5|셀6|셀7|셀8
셀9|셀10|셀11|셀12

테이블 정렬

헤더1|헤더2|헤더3
:---|:---:|---:
Left|Center|Right
1|2|3
4|5|6
7|8|9

## 12. Line Breaks 줄바꿈
* `<br>` 로 줄바꿈
### 줄바꿈 Syntax
    Sentence 1
    and this this is sentence 2
    Sentence 3 <br>
    and this this is sentence 4
### 줄바꿈 실행결과
Sentence 1
and this this is sentence 2
Sentence 3 <br>
and this this is sentence 4
#### 참고 링크
[markdown_ko](https://github.com/jinkyukim-me/markdown_ko?tab=readme-ov-file)
