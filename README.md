# nlp

This is the readme of my NLP project


## NLP的项目有三大类
1 Question answering and machine reading comprehension <br/>
2 task-oriented dialogue system <br/>
3 fully data-drive conversation models and social bots <br/>

该项目意在实现第二类任务，也就是task-oriented dialogue system（任务导向的对话系统） <br/>

该系统通常 分为四个模块

a) NLU(natural language understanding) <br/>
b) DST(dialogue state tracker)         --DM(Dialogue Manager) <br/>
c) POL(dialogue policy)                --DM(Dialogue Manager) <br/>
d) NLG(natural language generation) <br/>


## NLU
1) Intent classification implement on CrossWOZ <br/>
2) Slot extraction <br/>
3) Joint slot-intent <br/>


1) Intent classification/意图识别
通过bert将自然语言进行embeding，进行空间映射到向量空间
再用embedding的信息进行分类，看属于哪一类或者哪几类

通常分为single intent和multi intents 类别  
单分类任务使用 cross entropy；
多分类任务使用binary cross entropy（BCE）
作为损失函数

2) Slot extraction/把意图做需要的slot 标注出来
用bert做embedding

3) Joint slot-intent/把上面两件事同时做  

### bert motivation  
-- unlabeled corpra  
-- word embedding models are gennerally shallow  
-- do not take context into account  
-- longer context dependency for QA  
-- transfer learning  


## DST (dialogue state tracker)


## POL (dialogue policy)


## NLG (natural language generation)

## Bert motivation

unlabeled corpra <br/>
word embedding models are generally not very powerful, they are very shallow <br/>
dont take context into account <br/>
longer context dependency for QA <br/>
transfer learning <br/>
