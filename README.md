# test
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Watson TV</title>
    <meta name="description" content="">
    <meta name="viewport" content="width=device-width">

    <!-- Latest compiled and minified CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">

    <link rel="stylesheet" type="text/css" href="https://rawgit.com/ibm-early-programs/watson-tv/master/style.css">
    <link rel="stylesheet" type="text/css" href="https://rawgit.com/ibm-early-programs/watson-tv/master/fonts.css">
    <!-- <link rel="stylesheet" type="text/css" href="style.css"> -->
    <!-- <link rel="stylesheet" type="text/css" href="fonts.css"> -->
  </head>

  <body>
    <div class="tv-header">
      <div class="tv-container">
        <h1>
          LIVE
          <button class="btn tv-transcription-btn" onclick="tv.select('transcribe')">Transcription</button>
          <button class="btn tv-translation-btn tv-disabled-btn" onclick="tv.select('translate')">Translation</button>
        </h1>
        <i class="fa fa-dot-circle-o fa-2x" aria-hidden="true"></i>
      </div>
    </div>
    <div class="tv-tv">
      <div class="tv-container">
        <video id="tv-video" type="video/mp4">
          Your browser doesn't support HTML5 video tag.
        </video>

        <div class="tv-url">
          <span class="input-group">
            <span class="input-group-addon">URL</span>
            <input type="text" class="form-control" id="tv-url" placeholder=".mp4 URL, eg. TED Talk" value="https://r2---sn-25ge7nsl.googlevideo.com/videoplayback?itag=22&requiressl=yes&mime=video%2Fmp4&source=youtube&signature=BE37539F5E08A16029A7C52AABECBE3E97A945D3.D836254AE84E52979DE90474FCAD1C4A6E86257B&ei=nj4yW-yAKZuV1gb68ovgCw&ms=au%2Crdu&mt=1530019386&pl=17&usequic=no&expire=1530041086&ratebypass=yes&id=o-APXQTNSdSEf1pl1omL_HXyOveOo4VahvLs-K775PepKp&c=WEB&fvip=2&sparams=dur%2Cei%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpl%2Cratebypass%2Crequiressl%2Csource%2Cusequic%2Cexpire&ip=163.172.13.245&fexp=23709359&mm=31%2C29&dur=331.929&mv=m&lmt=1529892959370650&key=yt6&initcwndbps=321250&ipbits=0&mn=sn-25ge7nsl%2Csn-25glenes&type=video%252Fmp4%253B%2Bcodecs%253D%255C%2522avc1.64001F%252C%2Bmp4a.40.2%255C%2522&quality=hd720&title=American%2BMedia%252C%2BSoviet%2BTactics">
          </span>

          <button type="button" onclick="tv.sendUrl()" class="btn btn-default">Load</button>
        </div>
      </div>
    </div>
    <div class="tv-translation">
      <p id="tv-translation-text"></p>
    </div>
  </body>

  <script src="https://use.fontawesome.com/bc434e1504.js"></script>
  <script src="https://code.jquery.com/jquery-3.1.0.min.js" integrity="sha256-cCueBR6CsyA4/9szpPfrX3s49M9vUU5BgtiJj06wt/s=" crossorigin="anonymous"></script>

  <!-- Latest compiled and minified JavaScript -->
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
  <!-- <script src="scripts.js"></script> -->
  <script src="https://rawgit.com/ibm-early-programs/watson-tv/master/scripts.js"></script>
</html>
