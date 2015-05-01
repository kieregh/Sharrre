# SNS Share Widgets for [kimsq/Rb] (http://github.com/kimsq/rb)
kimsQ/Rb 기반 SNS 공유 위젯 -  [jQuery Sharrre Plugin] (http://www.sharrre.com) 응용.

## Features

## Requirment
1. 아래의 파일이 있어야 합니다. (구글+ 연동시 필요).

  ./plugins/sharrre/1.3.5/sharrre.php   
  만약 없으면 [여기서] (https://github.com/kimsQ/rb/commit/232a493499f9b83b199e9546ddd374bfffd6dafb)
  다운받아 서버의 해당 폴더에 업로드 해주세요.

2. 서버에 curl 이 설치되어 있어야 합니다.  

## Getting Started
1. [kimsQ Rb2] (http://www.kimsq.com) 설치(서버에 curl 익스텐션 필요). 
2. 위젯 설치 파일 다운로드
3. 킴스큐 관리자 모드 > 위젯 설치 버튼 > 2.에서 다룬로드 받은 설치파일 선택 
4. ```<head></head>``` 안에 아래의 메타태그 추가(각 SNS 렌더링 최적화). 
  
```   
    <link href="<?php echo strip_tags($g['url_root'].$_SERVER['REQUEST_URI'])?>" rel="canonical">
    <!-- Open Graph data for Facebook -->
    <meta property="og:type" content="article" />
    <meta property="og:url" content="<?php echo strip_tags($g['url_root'].$_SERVER['REQUEST_URI'])?>" />
    <meta property="og:title" content="<?php echo strip_tags($g['meta_tit'])?>" />
    <meta property="og:description" content="<?php echo strip_tags($g['meta_des'])?>" />
    <meta property="og:image" content="<?php echo strip_tags($g['meta_img'])?>" />
    <!-- Schema.org markup for Google+ -->
    <meta itemprop="name" content="<?php echo strip_tags($g['meta_tit'])?>">
    <meta itemprop="description" content="<?php echo strip_tags($g['meta_des'])?>">
    <meta itemprop="image" content="<?php echo strip_tags($g['meta_img'])?>"> 
    <!-- Twitter Card data -->
    <meta name="twitter:card" content="summary"/>
    <meta name="twitter:url" content="<?php echo strip_tags($g['url_root'].$_SERVER['REQUEST_URI'])?>"/>
    <meta name="twitter:title" content="<?php echo strip_tags($g['meta_tit'])?>" />
    <meta name="twitter:description" content="<?php echo strip_tags($g['meta_des'])?>" />
    <meta name="twitter:image:src" content="<?php echo strip_tags($g['meta_img'])?>" />
```
보다 자세한 내용은 [여기](http://www.kimsq.co.kr/market/785/) 를 참고해주세요.

기타 문의사항은 [이슈](https://github.com/kieregh/Sharrre/issues)에 등록해주세요.
 
감사합니다.

