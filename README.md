# Google-Class-Room-API-LINE-Bot

```gs
//======================================

      権限関係でボツになったBotです
          2022の7月に作りました

//======================================

function getClasses() {

  var response = Classroom.Courses.Announcements.list(ID).announcements;

    var time = [response[0].creationTime]; // 投稿時間
    // 時間の時差,フォーマットの変更
    var time = new Date(time).toLocaleString();
    var time = new Date(time);
    var timeHour = time.getHours();
    var timeHour = ('00' + timeHour).slice(-2);
    var timeMin = time.getMinutes();
    var timeMin = ('00' + timeMin).slice(-2);


var createTime = [response[0].creationTime];
        var createTime = new Date(createTime);
        var createTime = createTime.getTime();
        // 現在時刻の取得&変換
        var nowTime = new Date();
        var nowTime = nowTime.toGMTString();
        var nowTime = new Date(nowTime);
        var nowTime = nowTime.getTime();

var nc3 = nowTime - createTime;

let text1;

if (nc3 >= 30000) {

text1 ='古い投稿';

  }else{
    text1 = '新しい投稿';
  }
}

// LINE　API
//この下は見せられないよ！！！

```
