

الفصل دا بيتكلم عن حاجة اسمها الـRandom Variables ودي حاجة مهمة جداً في اﻹحصاء وظيفتها بإختصار تحولي النتائج بتعت التجارب ﻷرقام علشان يسهل التعامل معاها.
Function that assign a real number to every out come.
مثال، قلبنا عملة معدنية مرتين فايه النتائج الي هتطلع؟
S = {HH,HT, TH, TT}
دور الـRV بقى هو انا بدل ميطلعلك الي انا كاتبه دا يطلعلك أرقام، بناء على معادلة أو قاعدة معينة زي:
Let X is the numer of heads.

| S   | HH  | HT  | TH  | TT  |
| --- | --- | --- | --- | --- |
| x   | 2   | 1   | 1   | 0   |
فتبقى الـOut comes بتعتي هي الـ 0,1,2 وببدأ اتعامل بقى معاها بالشكل دا.
حاجة تانية مهمة بقى الـRV دا ممكن يتعمل للنوعين بتوع الـOutcomes الي هما Discrete or Contioue 

طيب طلعنا نتايج العينة وحولناها لـRV ازاي نطلع الإحتمالية P بتاعتها؟
الموضوع دا بطريقتين بحاجتين:
1- Probability Mass Function f(x) or P(X=x)
2- Cumulative Distribution Functions

## Probability Mass Function

The function that gives the probability of each value of a discrete random variable
ورمزها هو f(x) or P(X=x)
ودي ليها  ٣ شروط علشان أقول ان الـP جايه بالطريقة دي:
- P(X=xi​)≥0
- i∑​P(X=xi​)=1
- P(X=x)=0
هنبدأ نطبق الكلام دا على المثال الي فوق 


| x            | 0   | 1   | 2   |
| ------------ | --- | --- | --- |
| f(x), P(X=x) | 1/4 | 2/4 | 1/4 |
ولو بصيت هتلاقيهم محققين كل الشروط التﻻتة الي فوق.
## Cumulative Distribution Functions (CDFs)
gives the probability that **XXX is less than or equal to** a certain value x
F(x)=P(X≤x)
فتطبيقا على الجدول الي فوق لو انت عايز احتمالية x=2 فهي هتساوي مجموع احتماليات كل الـRV الي أقل من اتنين يعني هتساوي ربع + ربعين + ربع يعني هتساوي ١

| x            | 0   | 1   | 2   |
| ------------ | --- | --- | --- |
| f(x), P(X=x) | 1/4 | 2/4 | 1/4 |
| F(x), P(X≤X) | 1/4 | 3/4 | 1   |

طيب زي الفل الكلام دا كان عندنا Discrete Outcomes عملنالها Random Variable وبعدين جبنا الإحتمالية بتعت كل واحد فيهم، دلوقتي جه الدوء نجيب حاجتين مهمين جدا هما:

## Mean and Variance of a discrete random variabl
على طول في قوانين هتحكمنا هنا وهي 
1. Mean (Expected Value)
		E(X)=μ=∑[xi​⋅P(X=xi​)]
		مجموع ضرب المتغير في اﻹحتمالية بتعته

نطبق على المثال الي فوق دا:
	E(X) = 0 . 1/4 + 1 . 2/4 + 2. 1/4 = 1

2. Variance
		Var(X)=∑[(xi​−μ)2⋅P(X=xi​)]
		طرحنا القيمة من المتوسط وربعناها، وبعدين ضربناها في احتماليتها ثم جمعنا كل دا 
3. Standard Deviation
زي مانت عارف بناخد الجذر التربيعي للـVariance
4. Distribution
ودا عندنا منه أنواع كتير 
		1. Discrete Uniform Distribution
		2. Binomial Distribution
		3. Geometric Distribution
		4. Negative Binomial Distribution
		5. Hypergeometric Distribution
		6. Poisson Distribution

## Discrete Uniform Distribution  
بقول إن الـRV ليه النوع دا من التوزيع لما إحتمالية كل قيمة من قيمة تكون متساوية
مثال 
Let X = anything
n= values of X = {0,1,2} 
f(x!)=1/n

## Binomial Distribution
في حاجة إسمها Bernoulli trail ودي تجربة بتطلع حاجتين بس، صفر وواحد، نجاح وفشل، صح وخطأ
فلو التجربة دي عندي وتحقق فيها الشروط دي:
- trail are independant
- two possible outcome
- P remain constant 
X= number of trail that result success
وفي طبعا قانون تقدر تجيب منه Probability Mass Function, Mean and variance
## Geometric Distribution
نفس رقم ٢ لكن
X = number of trail to get the first success outcome
وفي قانون يجيبلك الـ٣ حاجات بتوع كل مرة
## Negative Binomial Distribution
نفس فكرة الي قبلها لكن
N = number of trails until r number of success occur
وطبعا هتكتب القوانين بتعتك
## Hypergeometric Distribution
هنا هنفرض إن عندنا عدد معين من الـObjects رمزه N
لو افترضنا ان جوه المجموعة دي عدد معين بيمثل الـSuccess رمز K والفشل N-K
فلو خدت عينه n 
N = number of success in the sample 
## Poisson Distribution
هنا بتعتمد على حاجة اسمها Poisson Process ؟؟
فبيقولك بقى 
N = number of events in a poisson
ونفس القوانين هتكتبها 