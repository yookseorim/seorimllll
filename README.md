# seorimllll
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>종민이랑 놀지마</title>
    <script>
        let dislikeCount = 0;

        function showPrompt() {
            const userChoice = confirm("종민이랑 놀지말라고\n확인을 누르면 '알았어', 취소를 누르면 '싫어'입니다.");
            if (userChoice) {
                alert("진작에 말들어야쥥!!  이거 짱재밋쥬 ㅋㅋㅋ");
            } else {
                dislikeCount++;
                handleDislike();
            }
        }

        function handleDislike() {
            if (dislikeCount === 1) {
                alert("응 그거아니야 다시선택해");
                showPrompt();
            } else if (dislikeCount === 2) {
                alert("그거아니라니까?");
                showPrompt();
            } else if (dislikeCount >= 3) {
                alert("니맘대로해 ㅡㅡ ㄲㅈ");
            }
        }
    </script>
</head>
<body onload="showPrompt()">
</body>
</html>
