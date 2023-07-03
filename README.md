# happybirthday-eunbean
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>은빈이에게</title>
    <!-- 맨위에 홈페이지 책갈피? 부분에 나타나는 문자 -->
    <link rel="shortcut icon" href="https://cdn2.iconfinder.com/data/icons/christmas-46/64/christmas-icon-tree-512.png">
    <!-- 트리아이콘 변경해야함!! -->

    <meta property="og:image"
        content="https://www.momswhothink.com/wp-content/uploads/christmas_gift_ideas_2012.jpg">
    <meta property="og:title" content="은채가">
    <meta property="og:description" content="19번째 생일을 축하하며">
    <!-- og태그 넣는 코드입니다. 링크를 보낼 때 미리보기 창 같은건데 거기에 나오는 이미지와
    제목, 간단한 내용을 첨부할 수 있습니다. -->

    
    <!-- 아래 링크는 폰트를 변경할 때 복사해서 붙여넣고 또 그 아래 <style>에도 붙여넣어준다. -->
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css2?family=Poor+Story&display=swap" rel="stylesheet">
    <style>
        * {
            font-family: 'Poor Story', cursive;
            /* 이 것이 폰트 변경할 때 붙여 넣어주는 코드 */
        }

        body {
            background-color: #86a18b;
            /* 홈페이지 배경 컬러를 빨간색으로 지정하는 코드 */
        }

        .envelope {
            /* 아래 클래스 지정한걸 불러와 꾸며준다. */

            width: 200px;
            height: 200px;
            /* 불러온 사진의 크기를 정하는 코드 */

            background-image: url(https://pngimg.com/uploads/envelope/envelope_PNG18366.png);
            background-size: cover;
            background-position: center;
            /* 이미지를 불러오고 화면에 나타나는 이미지 중앙을 맞춰주는 코드
            사진을 홈페이지 중앙에 맞추는 코드가 아니라 사진이 짤려서 나오는데
            해당 사진이 전체적으로 다 나오도록 만들어 주는 코드이다. */

            margin: 200px auto 0px auto;
            /* 봉투를 중앙으로 가져오기 위한 코드
            이 설정으로 좌측 상단에 위치한 봉투 사진을 중앙으로 데려왔다. */

            cursor: pointer;
            /* 마우스를 가져다 대면 마우스 포인터가 손 모양으로 바뀐다. */
        }

        .envelope-msg {
            /* 아래서 envelope-msg클래스를 만들었으니 여기서 불러와서 수정한다.  */
            color: white;
            /* 글자 색상을 흰 색으로 지정하는 코드 */

            text-align: center;
            /* 글자를 만들면 좌측 중앙에 치우쳐져 있는데 해당 코딩으로
            글자를 센터로 가져온다. */
        }

        .letter-close {
            display: block;
        }

        /* html 코드를 안 보이도록 설정해 주는 코딩 아래서 letter-close 클래스를 만들어
        위에 코딩한 기록 전체를 넣었다. 한 마디로, lerrer-close 클래스에 속하는 코딩을 감춰
        주는 기능. */

        .letter-open {
            display: none;
        }

        h1 {
            /* style에서 꾸미려면 클래스를 만들어야 하지만 해당 코딩에서 한 번밖에 사용을 안 하는
            코드는 바로 불러와서 사용해도 된다. h1을 1회만 사용할 거기 때문에 따로 클래스를 만들지 않아도 됨. */
            color: white;

            text-align: center;

            margin-top: 30px;
            margin-bottom: 30px;
            /* 글자 위, 아래 공간을 조절하는 코딩 */
        }

        .messgebox {
            background-color: rgb(223, 255, 232);

            width: 400px;
            margin: auto;

            color: rgb(34, 73, 50);

            padding: 30px;
            /* 안쪽으로의 여백 */
            font-size: 20px;
            /* 폰트 사이즈 변경하는 코드 */
            line-height: 20px;
            /* 줄 바꿈 사이 간격 ( 엔터키 눌렀을 때 아래로 쓰이는 것이 줄 바꿈) */
            box-shadow: 0px 0px 10px 0px rgb(253, 221, 221);

        }

        .from {
            text-align: right;
            /* from 클래스를 우측 정렬으로 만드는 코딩 */
            margin-bottom: 0px;
            /* 아래 공간을 줄여주는 코딩.글자 아래 공간이 길쭉하게 생기는걸 줄여준다. */

        }

        @media screen and (max-width: 760px) {

            /* 모바일 처리하는 코딩 */
            .messgebox {
                width: 300px;

                padding: 20px;
            }

            /* 위에 설정은 max-width: 760px아래일 때만 실행해라.
            넓이가 760이면 패드나 폰 종류에서만 실행되고 노트북 같이 길이가 넓게
            출력이 되는 화면에서는 실행이 되지 않는다. */
            .rtan {

                width: 150px;
                height: 150px;
                margin: 70px auto 0px auto;

            }

            h1 {
                font-size: 28px;
            }

            .envelope {

                margin: 150px auto 0px auto;

            }

            /* 아래 <script>를 만들어 Javascript 버튼을 만들어준다. open_letter()이걸 복사하여 아래 body-div에 편지봉투
    란에 붙여넣어 줬다. 스크립트 위아래로 주석을 달면 화면에 보여서 여기에 쓴다. */
            /* 아래 자바 스크립트 참고 go_rtan()는 히든 메시지와 함께 링크로 이동하게 되는 코딩이다. 마찬가지로 rtan에 가서 
    붙여넣기로 go_rtan()이걸 넣어 함수를 만들고 실행한다. */
    </style>

    <script>

        function open_letter() {
            document.getElementsByClassName("letter-close")[0].style.display = 'none'
            document.getElementsByClassName("letter-open")[0].style.display = 'block'
        }

        function go_rtan() {
            alert('하이')
            window.location.href = 'https://ohjuhyeon.tistory.com/';
        }

    </script>

</head>

<body>
    <div class="letter-close">
        <div class="envelope" onclick="open_letter()"></div>
        <!-- url을 넣어 편지 봉투를 홈페이지에 나타나게 하기 위해 envelope 클래스를 만들어준다. -->
        <h2 class="envelope-msg">클릭해보던가말던가</h2>
        <!-- 봉투 아래에 택스트를 넣기 위해 envelope-msg 클래스를 만들었고 위에서 불러와 수정. -->
    </div>

    <div class="letter-open">
        <div class="rtan" onclick="go_rtan()"></div>
        <h1>19th Birthday</h1>
        <div class="messgebox">
            글자수 테스트 ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ <br />
            첫줄 ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ<br />
            둘째줄ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ <br />
            세째줏둘 ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ<br />
            넷째줄ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ <br />
            <p class="from">2023.7.6 MADE BY 고은채</p>
        </div>
    </div>


</body>

</html>
