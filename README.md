# philo_shl13_execute
execute version of philosophers 42 shl13. no code 


### 1. TEST CASE
- 200 필로소퍼 이상 테스트 하지 말아라
- time_to_die, time_to_eat, time_to_sleep을 60ms 이하로 테스트 하지 말아라
- 1 800 200 20으로 테스트하고 먹지 않고 주어야 한다. (7월 업데이트로 추가된 내용)
- 5 800 200 200으로 테스트 하고 아무도 죽으면 안된다.
- 5 800 200 200 7로 테스트하고 철학자가 7번 식사를 하면 멈춰야 한다.
- 4 410 200 200으로 테스트 아무도 죽으면 안된다
- 4 310 200 100 ⇒ 한 명의 철학자가 죽는다
- 2명의 철학자를 이용해서 다른 시간으로 테스트 해봐라. (죽음 딜레이가 10ms를 넘어서는 것은 안된다)
- 각자의 값으로 테스트 해봐라 제 때 철학자들이 죽는지 포크를 빼앗지 않는지 등등
<br/> 

### 2. Socrates tester test case
- 4 311 150 150 no death (Even number test)
- 5 600 150 150 no death (Odd number test)
- 3 310 200 100 yes death (Death timing test)


<br/> 

### 3. 체크해볼만한 내용 
- norminette
- leaks 
- 10ms delay 
- 1명일 때 제대로 출력하고 죽는지. (0ms 1 has taken a fork. 802 1 died.) 
- 세마포어와 뮤텍스의 차이 (보너스까지 했다면)
- 프로세스와 스레드의 차이 (보너스까지 했다면)        
    
<br/> 
      

### 4. 2021년 7월 업데이트로 달라진 점 
[PHILOSOPHERS]
- Remove multi-thread with semaphore.
- Move muti-process with semaphore to bonus part.
- If there is just one philosopher, it must die.     


philo_one -> philo

philo_three -> philo_bonus

philo_two -> X
