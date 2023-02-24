# Article_rec

한국어 뉴스 추천서비스를 위한 NLP 모델 테스트

NLP 모델을 통해 기사를 벡터화 후 코사인유사도를 통해 기사 간 유사도를 비교

# Test model list
word2vec

KoBERT

KR-SBERT

BERT(BERT4DOC)

KoELECTRA

# Results

정량평가 결과

<img width="417" alt="image" src="https://user-images.githubusercontent.com/76480887/220228999-98d20237-f23a-4997-9e25-880237462e64.png">

정성평가 결과

<img width="920" alt="image" src="https://user-images.githubusercontent.com/76480887/220229128-dfffe0db-89fd-42d1-bebb-9818050ad90a.png">

타 모델에 비해 SBert가 문맥적인 이해가 뛰어났으며 타겟에 유사한 내용의 기사를 추천하였다
