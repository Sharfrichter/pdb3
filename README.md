# Лабораторная работа №3

В качестве предметной области выбраны животные у каждого из них есть название и масса, а также принадлежность к млекопитающим либо рептилиям, и травоядным или плотоядным.

## Команды для создания сущностей

CREATE  
(tiger:animal{name:"тирг",weight:300}),      
(crocodile:animal{name:"крокодил",weight:500}),   
(cobra:animal{name:"кобра",weight 3}),          
(elephant:animal{name:"слон",weight:6000}),  
(giraffe:animal{name:"жираф",weight:800}),  
(horse:animal{name:"лошадь",weight:800}),  
(herbivorous:eating{name:"травоядное"}),  
(carnivorous:eating{name"плотоядное"}),  
(mammal:class{name:"млекопитающее"}),  
(reptile:class{name:"рептилия"}),  
(tiger)-[:eating{name:"питание"}]->(carnivorous),  
(crocodile)-[:eating{name:"питание"}]->(carnivorous),  
(cobra)-[:eating{name:"питание"}]->(carnivorous),  
(elephant)-[:eating{name:"питание"}]->(herbivorous),  
(giraffe)-[:eating{name:"питание"}]->(herbivorous),  
(horse)-[:eating{name:"питание"}]->(herbivorous),  
(tiger)-[:belong{name:"принадлежать"}]->(mammal),  
(elephant)-[:belong{name:"принадлежать"}]->(mammal),  
(giraffe)-[:belong{name:"принадлежать"}]->(mammal),  
(horse)-[:belong{name:"принадлежать"}]->(mammal),  
(cobra)-[:belong{name:"принадлежать"}]->(reptile),  
(crocodile)-[:belong{name:"принадлежать"}]->(reptile)  

## Команды для поиска в базе
