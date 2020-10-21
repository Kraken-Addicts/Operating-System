
## 6장 CPU 스케줄링

<br>

### 6-1 :fallen_leaf: CPU 스케줄러　`yeosong`
 
문제 작성


<details>
<summary> <b> :page_facing_up: 답지 </b>  </summary>
<div markdown="1">
 
답 작성 

</div>
</details>
<br><br>

### 6-2 :fallen_leaf: 디스패처	　`kukim`
 
1. 디스패처(dispatcher)이란 무엇인가요? (주관식)  

2. 디스패치 지연시간(dispatch latency)이란 무엇인가요? (주관식)  

3. 디스패치 지연시간의 대부분은 어디에 해당될까요? (보기 선택)
```
보기 : 파파라치 사진찍기, 오버헤드킥, 문맥교환 오버헤드, PCB I/O,  CPU bound process
```

4. 다음은 디스패처의 수행 작업 과정이다. 보기에서 괄호를 채우시오.

```
보기 : PC, SP, PCB, 디스패치, 찰칵찰칵, SD 카드
```

현재 수행중이던 프로세스의 문맥(context)을 그 프로세스의 (   )에 저장하고

새롭게 선택된 프로세스의 문맥을 (   )로부터 복원한 후 그 프로세스에게 CPU를 넘기는 과정을 수행한다.

<details>
<summary> <b> :page_facing_up: 답지 </b>  </summary>
<div markdown="1">
 
1. 디스패처(dispatcher)이란 무엇인가요? (주관식)  
정답 : CPU 스케줄러가 어떤 프로세스에게 CPU를 할당해야 할지 결정하고나면 선택된 프로세스에게 실제로 CPU를 이양하는 작업이 필요한데 이때 새롭게 선택된 CPU를 할당, 작업 수행할 수 있도록 환경설정 하는 운영체제의 코드이다.

2. 디스패치 지연시간(dispatch latency)이란 무엇인가요? (단답형)  
디스패처가 하나의 프로세스를 정지시키고 다른 프로세스에게 CPU를 전달하기까지 걸리는 시간

3. 디스패치 지연시간의 대부분은 어디에 해당될까요?
```
보기 : 파파라치 사진찍기, 오버헤드킥, 문맥교환 오버헤드, PCB I/O,  CPU bound process
```
정답 : 문맥교환 오버헤드

4. 다음은 디스패처의 수행 작업 과정이다. 괄호를 채우시오.

```
보기 : PC, SP, PCB, 디스패치, 찰칵찰칵, SD 카드
```

현재 수행중이던 프로세스의 문맥(context)을 그 프로세스의 (PCB)에 저장하고

새롭게 선택된 프로세스의 문맥을 (PCB)로부터 복원한 후 그 프로세스에게 CPU를 넘기는 과정을 수행한다.
</div>
</details>
<br><br>


### 6-3 :fallen_leaf: 스케줄링의 성능 평가	　`gaekim`
 
문제 작성


<details>
<summary> <b> :page_facing_up: 답지 </b>  </summary>
<div markdown="1">
 
답 작성 

</div>
</details>
<br><br>

### 6-4 :fallen_leaf: 스케줄링 알고리즘	　`mihykim`
 
문제 작성


<details>
<summary> <b> :page_facing_up: 답지 </b>  </summary>
<div markdown="1">
 
답 작성 

</div>
</details>
<br><br>

### 6-5 :fallen_leaf: 스케줄링 알고리즘의 평가 	　`daelee`
 
- 스케줄링 알고리즘의 성능을 평가하는 방법으로는 `____`, `____`, `______` 방식이 있다.

  ```
  보기 : 시뮬레이션, 뿌잉모델, 트레이스(trace), 구현, 나현, 다현, 대현, 실측, 로드 타임 바인딩, 큐잉모델, 세그먼테이션 기법, 구현 및 실측, 페이징, 고정분할
  ```


<details>
<summary> <b> :page_facing_up: 답지 </b>  </summary>
<div markdown="1">

- 스케줄링 알고리즘의 성능을 평가하는 방법으로는 `____`, `____`, `______` 방식이 있다.

  ```
  시뮬레이션, 뿌잉모델, 트레이스(trace), 구현, 나현, 다현, 대현, 실측, 로드 타임 바인딩, 큐잉모델, 세그먼테이션 기법, 구현 및 실측, 페이징, 고정분할
  ```

  > 정답 : 큐잉모델, 시뮬레이션, 구현 및 실측
  >
  > - **큐잉모델(que-ueing model)** : 확률분포를 통해 프로세스의 도착률과 cpu 처리율을 입력값으로 준 뒤 각종 성능지표(cpu의 처리량, 프로세스의 평균 대기시간 등)를 구하는 방식
  > - **구현 및 실측(implementation & measurement) :** 운영체제 커널의 cpu 스케줄링 코드를 수정해, 동일한 프로그램을 원래 커널과 수정한 커널에서 수행시켜보고 실행시간을 측정/비교하는 방식
  > - **시뮬레이션(simulation) :** 가상으로 cpu 스케줄링 프로그램을 작성해 결과를 확인하는 방식. 입력값은 실제 시스템에서의 cpu 요청내역을 추출해 사용하기도 하는데, 이 값을 `트레이스(trace)`라고 부른다.

  

</div>
</details>
<br><br>
