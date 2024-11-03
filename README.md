# transformer encoder NLP-portfolio
자연어, 생성형 , 강화학습 ai 포트폴리오

1) transformer encoder로 동의어 관계 분석 , 위의 transformer_partially_complete이 해당 파일임.
   
   epoch : 99, train_loss : 0.43970897793769836 , test_dataset : {'accuracy': 0.664927536231884, 'f1': 0.7987465181058496}(별도의 scheduling이나 checkpoint지정은 하지 않고 train dataset에 epoch100으로만 훈련함)
   
   pretrained transformer encoder model 쓰지 않음
   
추가 실험 예정

https://github.com/genji970/NLP-LLM-portfolio-save/blob/main/transformer_partially_complete.ipynb

2) llm start
   i) ibm-granite/granite-3.0-8b-instruct 사용 , fine tuning을 하기 위한 구조가 갖추어졌는지 확인용으로 훈련데이터는 1개만 만들어 입력,

구현 과정 : 
   autotokenizer로 token 생성(pad = 0), AutoModelForCausalLM 사용, model freeze하고 Lora 사용(저차원 = 8), model -> peft처리된 model, tokenized data 생성 , train , 3epoch만 돌렸고 train loss는 굉장히 큼. tensorboard로 결과 시각화

3) soft actor critic mujoco half cheeath
   https://github.com/genji970/soft-actor-critic
   
4) rl paper study
https://github.com/genji970/RL-stock-prediction-paper-study

. 수학 : 해석학 , 선대 , 테일러급수 등
