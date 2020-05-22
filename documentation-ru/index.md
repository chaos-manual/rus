# zzz

## О чем здесь речь

We document a chaos engineering (CE) process the way it 
can work in an industrial-grade practice. 

## Где применяется 

In our opinion CE is most relevant for:

- highload projects (benefits > cost of implementation)
- actively maintained (you can both detect and fix a vulnerability)
- distributed system (fewer things break in a monolith)
- ready mindsets (the team attaches value to system reliability and is willing to allocate time and resources to keep it up)

Не очень подходит для маленьких компаний с 4 разработчиками
(изучать можно, но на маленькой ИТ-системе выигрыши будут небольшие).

## Для кого это руководство

Novice. We fully describe a battle-tested implementation 
and give our reasoning why it works well. This should be 
a good starting point for those just introducing 
or experimenting with chaos engineering. Please 

Expert. Next, we provide recommendations for more advanced 
users, based on your feedback and questions.

## О разделах

The core of our manual is CE [process description](process.md). It outlines the starting points and outcomes of chaos engineering and relations of CE to other software engineering/devops/business processes.

The [injections section](injections.md) is a body of knowledge that helps 
to categorise vulnerabilities, design tests. we also offer a few 
examples and common patterns to fix your system.

We also maintain a [glossary](glossary.md) of terms to help 
navigate terminlogy and some specific CE slang more easily.

## Наш подход

Things we present are not dark magic. They are not about 
buying into any expensive stuff. They are about sensible steps 
in acquiring competences and changing your workflow. As a result 
your IT system is more reliable and your team gets more confident 
and prepared.

Getting more 9's is a journey, not a single act, so let's start!

## Авторы

This manual is written by [Dmitry Yakubovsky (Sberbank)](https://twitter.com/d_yakubovsky) 
and [Evgeniy Pogrebnyak (MGIMO)](https://twitter.com/PogrebnyakE).  
