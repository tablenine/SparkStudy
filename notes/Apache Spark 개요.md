## Apache Spark 개요

+ BlinkDB
+ 다양한 기술들을 하나의 방법으로 처리하기 위함
+ Microsoft Dryad Paper를 기반으로 개발
+ In-Memory Architecutre
+ MapReduce에 비해 10배(disk) ~ 100배(memory) 의 성능
+ Hadoop과 완벽하게 호환
+ RDD(Resilient Distributed Dataset)
  + Spark의 핵심 추상화 기법
  + 변경불가능, 재생성, 에러복구가 가능한 여러 파티션으로 나누어 저장 된 레코드들의 컬렉션
  + 클러스터 노드들 사이에 파티션을 표현
  + Data Set의 병렬 처리를 가능하게 함
  + 파티션은 메모리나 디스크에 존재