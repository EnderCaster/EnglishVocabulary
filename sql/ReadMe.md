# Vocabulary Table
| Name | Type | Description |  
|------|------|-------------|
|id|int unsigned|primary key, make assosiation to other table|
|word|varchar||
|translation|varchar||
|description|varchar|A brief description for this word|
|image|text|the base64 code for other format data, that can take a scence of the word to your heart|

# Assosiation Table
| Name | Type | Description |  
|------|------|-------------|
|id|int unsigned|primary key,use it as dictiton type|
|dictionaryName|varchar|the name is unique|
|tableName|varchar|coresponding table name|
|description|varchar|short description|

# Dictionary Table
| Name | Type | Description |  
|------|------|-------------|
|id|int unsigned|just primary key|
|dictionaryId|int unsigned|foreign key,assosiation(id)|
|wordId|int unsigned|foreign key,vocabulary(id)|