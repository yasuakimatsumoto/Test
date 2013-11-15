FB.getLoginStatus(function(response) {
	if (response.session) {
	    //ログイン後の処理
	} else {
	   login()//ログインしてないのでログインしてもらう
	}
});
function login(){
	FB.login(function(response) {
	  if (response.session) {
	    if (response.perms) {
	      //ログイン後の処理
	    } else {
	      //パーミッション不許可。土下座しなくちゃダメですか(＞＜)
	    }
	  } else {
	    // ログイン失敗
	  }
	}, {perms:'read_stream,publish_stream,offline_access'});
}
