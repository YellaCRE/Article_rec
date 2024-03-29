# Article_rec

한국어 뉴스 추천서비스를 위한 한국어 임베딩 모델 테스트

한국어 임베딩 모델을 통해 기사를 벡터화 후 코사인유사도를 통해 기사 간 유사도를 비교

![자연어](https://user-images.githubusercontent.com/76480887/222945500-9ab0d330-4274-4dc0-88b4-f8c2ce8bff3b.png)

# Test model list
* word2vec
* KoBERT
* KR-SBERT
* BERT(BERT4DOC)
* KoELECTRA

# Results

KR-SBert
<img width="1006" alt="image" src="https://user-images.githubusercontent.com/76480887/221086285-c0911e90-d741-4491-81e5-82901d337ac2.png">


실험 결과

<img width="920" alt="image" src="https://user-images.githubusercontent.com/76480887/220229128-dfffe0db-89fd-42d1-bebb-9818050ad90a.png">

# Conclusions

타 모델에 비해 SBert가 문맥적인 이해가 뛰어났으며 타겟과 유사한 카테고리의 기사를 추천.  
실험초반, KoBert와 Bert4Doc의 성능이 SBert에 비해 나오지 않은 것을 각각 vocab의 수 부족과 한국어 vocab이 아닌 것으로 예상하였으나 
KoBert보다 vocab의 수가 압도적으로 많고 한국어 모델인 KoELECTRA를 실험했을 때도 결과가 좋지 못함.  
따라서 두 문장간의 유사도를 비교하는 실험에는 SBert의 성능이 뛰어남을 알 수 있음.
