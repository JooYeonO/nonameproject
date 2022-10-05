# nonameproject
## How to MangoDB
☑️ 포트 설정

$mongod --port 27017  //27017은 mangoDB기본 port


☑️ dbpath 설정

$mongod --dbpath C:\Users\Document\db('파일경로')


☑️ database 확인

$show dbs


☑️ db collection하기

$use manager('db명')

$db //db를 manager로 사용함
$db.createCollection("user")  //"user"라는 db를 생성
$show collections //user가 나타나면 잘 실행된 것

☑️ 데이터 insert하기(createCollection을 이용하지 않고 admin이라는 db를 바로 생성하기)
$db.admin.insertOne({name : "jooyeon"('JSON data')})   //insertOne : 한개의 데이터를 insert하겠다
JSON(JavaScript Object Notation) : 속성-값 쌍으로 이루어진 데이터 오브젝트를 전달하기 위해 인간이 읽을 수 있는 텍스트를 사용하는 개방형 표준 포맷
$show collections //admin출력

☑️ 입력한 데이터 확인하기
$db.admin.find()

☑️ 입력한 데이터 JSON형태로 정리하여 확인하기
$db.admin.find().pretty()

