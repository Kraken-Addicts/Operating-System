
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
 
문제 작성


<details>
<summary> <b> :page_facing_up: 답지 </b>  </summary>
<div markdown="1">
 
답 작성 

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
