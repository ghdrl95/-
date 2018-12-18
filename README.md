<html>

<head>
<meta http-equiv=Content-Type content="text/html; charset=ks_c_5601-1987">
<meta name=Generator content="Microsoft Word 14 (filtered)">

</head>

<body lang=KO>

<div class=WordSection1>

<p class=MsoNormal><b><span lang=EN-US style='font-size:12.0pt;line-height:
115%'>python</span></b><b><span style='font-size:12.0pt;line-height:115%'>의<span
lang=EN-US> django </span>모듈을 활용한 웹서버 구축</span></b></p>

<p class=MsoNormal><span lang=EN-US>Django</span>의 기능을 배울 때 이해하기 쉽도록 순차적으로 기능을 확장한
프로젝트를 폴더별로 구분</p>
<table border="0" cellpadding="0" cellspacing="0" style="border:1px solid #cccccc; border-left:0; border-bottom:0;" class="__se_tbl"><tbody>
<tr><td style="border-width: 0px 0px 1px 1px; border-bottom-style: solid; border-left-style: solid; border-bottom-color: rgb(204, 204, 204); border-left-color: rgb(204, 204, 204); border-image: initial; border-top-style: initial; border-top-color: initial; border-right-style: initial; border-right-color: initial; width: 467px; height: 17px; background-color: rgb(255, 255, 255);" class=""><p style="text-align: center; ">&nbsp;설치파일</p></td>
<td style="border-width: 0px 0px 1px 1px; border-bottom-style: solid; border-left-style: solid; border-bottom-color: rgb(204, 204, 204); border-left-color: rgb(204, 204, 204); border-image: initial; border-top-style: initial; border-top-color: initial; border-right-style: initial; border-right-color: initial; width: 467px; height: 17px; background-color: rgb(255, 255, 255);" class=""><p style="text-align: center; ">설치버전&nbsp;</p></td>
</tr>
<tr><td style="border-width: 0px 0px 1px 1px; border-bottom-style: solid; border-left-style: solid; border-bottom-color: rgb(204, 204, 204); border-left-color: rgb(204, 204, 204); border-image: initial; border-top-style: initial; border-top-color: initial; border-right-style: initial; border-right-color: initial; width: 467px; height: 17px; background-color: rgb(255, 255, 255);" class=""><p style="text-align: center; ">&nbsp;python</p></td>
<td style="border-width: 0px 0px 1px 1px; border-bottom-style: solid; border-left-style: solid; border-bottom-color: rgb(204, 204, 204); border-left-color: rgb(204, 204, 204); border-image: initial; border-top-style: initial; border-top-color: initial; border-right-style: initial; border-right-color: initial; width: 467px; height: 17px; background-color: rgb(255, 255, 255);" class=""><p style="text-align: center; ">3.6&nbsp;</p></td>
</tr>
<tr><td style="border-width: 0px 0px 1px 1px; border-bottom-style: solid; border-left-style: solid; border-bottom-color: rgb(204, 204, 204); border-left-color: rgb(204, 204, 204); border-image: initial; border-top-style: initial; border-top-color: initial; border-right-style: initial; border-right-color: initial; width: 467px; height: 17px; background-color: rgb(255, 255, 255);" class=""><p style="text-align: center; ">&nbsp;django 모듈</p></td>
<td style="border-width: 0px 0px 1px 1px; border-bottom-style: solid; border-left-style: solid; border-bottom-color: rgb(204, 204, 204); border-left-color: rgb(204, 204, 204); border-image: initial; border-top-style: initial; border-top-color: initial; border-right-style: initial; border-right-color: initial; width: 467px; height: 17px; background-color: rgb(255, 255, 255);" class=""><p style="text-align: center; ">2.x&nbsp;</p></td>
</tr>
<tr><td style="border-width: 0px 0px 1px 1px; border-bottom-style: solid; border-left-style: solid; border-bottom-color: rgb(204, 204, 204); border-left-color: rgb(204, 204, 204); border-image: initial; border-top-style: initial; border-top-color: initial; border-right-style: initial; border-right-color: initial; width: 467px; height: 17px; background-color: rgb(255, 255, 255);" class=""><p style="text-align: center; ">&nbsp;이클립스</p></td>
<td style="border-width: 0px 0px 1px 1px; border-bottom-style: solid; border-left-style: solid; border-bottom-color: rgb(204, 204, 204); border-left-color: rgb(204, 204, 204); border-image: initial; border-top-style: initial; border-top-color: initial; border-right-style: initial; border-right-color: initial; width: 467px; height: 17px; background-color: rgb(255, 255, 255);" class=""><p style="text-align: center; ">oxygen</p></td>
</tr>
<tr><td style="border-width: 0px 0px 1px 1px; border-bottom-style: solid; border-left-style: solid; border-bottom-color: rgb(204, 204, 204); border-left-color: rgb(204, 204, 204); border-image: initial; border-top-style: initial; border-top-color: initial; border-right-style: initial; border-right-color: initial; background-color: rgb(255, 255, 255);" class="" rowspan="1" colspan="1"><p style="text-align: center; ">&nbsp;pydev 플러그인</p></td><td style="border-width: 0px 0px 1px 1px; border-bottom-style: solid; border-left-style: solid; border-bottom-color: rgb(204, 204, 204); border-left-color: rgb(204, 204, 204); border-image: initial; border-top-style: initial; border-top-color: initial; border-right-style: initial; border-right-color: initial; background-color: rgb(255, 255, 255);" class="" rowspan="1" colspan="1"><p style="text-align: center; " align="center">마켓 플레이스에서 검색 후 다운&nbsp;</p></td></tr></tbody>
</table><p><br></p><p style="box-sizing: border-box; margin-bottom: 16px; color: rgb(36, 41, 46); font-family: -apple-system, BlinkMacSystemFont, &quot;Segoe UI&quot;, Helvetica, Arial, sans-serif, &quot;Apple Color Emoji&quot;, &quot;Segoe UI Emoji&quot;, &quot;Segoe UI Symbol&quot;; font-size: 16px; background-color: rgb(255, 255, 255);"><span style="box-sizing: border-box; font-weight: 600;">폴더 별 추가된 기능</span></p><p style="box-sizing: border-box; margin-bottom: 16px; color: rgb(36, 41, 46); font-family: -apple-system, BlinkMacSystemFont, &quot;Segoe UI&quot;, Helvetica, Arial, sans-serif, &quot;Apple Color Emoji&quot;, &quot;Segoe UI Emoji&quot;, &quot;Segoe UI Symbol&quot;; font-size: 16px; background-color: rgb(255, 255, 255);"><span lang="EN-US" style="box-sizing: border-box;">/project1 :&nbsp;</span>프로젝트 생성 후<span lang="EN-US" style="box-sizing: border-box;">&nbsp;bookmark&nbsp;</span>어플리케이션 생성<span lang="EN-US" style="box-sizing: border-box;">.&nbsp;</span>모델<span lang="EN-US" style="box-sizing: border-box;">,&nbsp;</span>뷰<span lang="EN-US" style="box-sizing: border-box;">,&nbsp;</span>템플릿 구조를 확인</p><p style="box-sizing: border-box; margin-bottom: 16px; color: rgb(36, 41, 46); font-family: -apple-system, BlinkMacSystemFont, &quot;Segoe UI&quot;, Helvetica, Arial, sans-serif, &quot;Apple Color Emoji&quot;, &quot;Segoe UI Emoji&quot;, &quot;Segoe UI Symbol&quot;; font-size: 16px; background-color: rgb(255, 255, 255);"><span lang="EN-US" style="box-sizing: border-box;">/project2 : django</span>튜토리얼 어플리케이션을 개발<span lang="EN-US" style="box-sizing: border-box;">(vote&nbsp;</span>어플리케이션<span lang="EN-US" style="box-sizing: border-box;">)</span></p><p style="box-sizing: border-box; margin-bottom: 16px; color: rgb(36, 41, 46); font-family: -apple-system, BlinkMacSystemFont, &quot;Segoe UI&quot;, Helvetica, Arial, sans-serif, &quot;Apple Color Emoji&quot;, &quot;Segoe UI Emoji&quot;, &quot;Segoe UI Symbol&quot;; font-size: 16px; background-color: rgb(255, 255, 255);"><span lang="EN-US" style="box-sizing: border-box;">/project3 : vote</span>어플리케이션 확장<span lang="EN-US" style="box-sizing: border-box;">&nbsp;(form&nbsp;</span>기반의 모델 객체 추가<span lang="EN-US" style="box-sizing: border-box;">/</span>수정<span lang="EN-US" style="box-sizing: border-box;">/</span>삭제<span lang="EN-US" style="box-sizing: border-box;">)</span></p><p style="box-sizing: border-box; margin-bottom: 16px; color: rgb(36, 41, 46); font-family: -apple-system, BlinkMacSystemFont, &quot;Segoe UI&quot;, Helvetica, Arial, sans-serif, &quot;Apple Color Emoji&quot;, &quot;Segoe UI Emoji&quot;, &quot;Segoe UI Symbol&quot;; font-size: 16px; background-color: rgb(255, 255, 255);"><span lang="EN-US" style="box-sizing: border-box;">/project4 : customlogin&nbsp;</span>어플리케이션 생성<span lang="EN-US" style="box-sizing: border-box;">&nbsp;(django</span>의 회원관리 어플리케이션을 바탕으로 회원가입<span lang="EN-US" style="box-sizing: border-box;">,&nbsp;</span>로그인<span lang="EN-US" style="box-sizing: border-box;">,&nbsp;</span>로그아웃 기능 추가<span lang="EN-US" style="box-sizing: border-box;">),&nbsp;</span>템플릿 확장기능으로 효율적으로<span lang="EN-US" style="box-sizing: border-box;">&nbsp;html&nbsp;</span>관리</p><p style="box-sizing: border-box; margin-bottom: 16px; color: rgb(36, 41, 46); font-family: -apple-system, BlinkMacSystemFont, &quot;Segoe UI&quot;, Helvetica, Arial, sans-serif, &quot;Apple Color Emoji&quot;, &quot;Segoe UI Emoji&quot;, &quot;Segoe UI Symbol&quot;; font-size: 16px; background-color: rgb(255, 255, 255);"><span lang="EN-US" style="box-sizing: border-box;">/project5 : blog&nbsp;</span>어플리케이션<span lang="EN-US" style="box-sizing: border-box;">(</span>게시판 형태의 어플리케이션<span lang="EN-US" style="box-sizing: border-box;">,&nbsp;</span>파일 및 이미지 업로드 기능을 사용할 수 있도록 모델 정의<span lang="EN-US" style="box-sizing: border-box;">)</span>과<span lang="EN-US" style="box-sizing: border-box;">social-auth-app-django&nbsp;</span>모듈 기반의 소셜로그인 기능 구현</p><p style="box-sizing: border-box; margin-bottom: 16px; color: rgb(36, 41, 46); font-family: -apple-system, BlinkMacSystemFont, &quot;Segoe UI&quot;, Helvetica, Arial, sans-serif, &quot;Apple Color Emoji&quot;, &quot;Segoe UI Emoji&quot;, &quot;Segoe UI Symbol&quot;; font-size: 16px; background-color: rgb(255, 255, 255);"><span lang="EN-US" style="box-sizing: border-box;">/project6 : blog&nbsp;</span>어플리케이션의 템플릿<span lang="EN-US" style="box-sizing: border-box;">,&nbsp;</span>뷰<span lang="EN-US" style="box-sizing: border-box;">,&nbsp;</span>검색 기능 추가</p>
</div>

</body>

</html>
