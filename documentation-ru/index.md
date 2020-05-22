# Введение

In this manual we document a chaos engineering (CE) process the way it 
can work in an industrial-grade practice. We provide failure
cases and patterns to fix them.

## Где применяется // Scope

CE done right has a great impact on reliability of highload 
IT services. But it is an advanced and costly technique.
There several things that have to be in place before CE
may strive, including proper monitoring and explicit reliability 
objectives.

In our opinion CE is most relevant for:

- highload projects (benefits > cost of implementation)
- actively maintained (you can both detect and fix a vulnerability)
- distributed system (fewer things break in a monolith)
- ready mindsets (the team attaches value to system reliability and is willing to allocate time and resources to keep it up)

Не очень подходит для маленьких компаний с 4 разработчиками
(изучать можно, но на маленькой ИТ-системе выигрыши будут небольшие).

Мы считаем, что уже знакомы с CE и заинтересованы в имплементации.
О вопросе CE или не CE - v10n.com

## Для кого это руководство

This manual is for those who practice chaos engineering
and have specific "How do I?" questions. We target the teams that have tried some fault injections 
and are not fully satisfied with the progress. 


We've been at that point and know the frustration of trying to pull too many pieces together and pressure to make complex decisions. The battle-tested solutions we came up to over few years are described in this manual. We hope they can be useful fo your chaos engineering team.

## Что внутри руководства

The core of our manual is CE [process description](process.md). It outlines the starting points and outcomes of chaos engineering and relations of CE to other software engineering/devops/business processes.

The [injections section](injections.md) is a body of knowledge that helps 
to categorise vulnerabilities, design tests. We offer a few 
examples and common patterns to fix your system.

We also maintain a [glossary](glossary.md) of terms to help 
navigate terminlogy and some specific CE slang.

## Особенности подхода

Things we present are not dark magic. They are not about 
buying into any expensive stuff. They are about sensible steps 
in acquiring competences and changing your own workflow
and interactions with other teams. 

Getting more 9's is a journey, not a single act, so let's start!

## Авторы

This manual is written by [Dmitry Yakubovsky (Sberbank)](https://twitter.com/d_yakubovsky) 
and [Evgeniy Pogrebnyak (MGIMO)](https://twitter.com/PogrebnyakE).  
