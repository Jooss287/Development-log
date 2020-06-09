
```
set CURPATH=%cd%
call "C:\Program Files (x86)\Microsoft Visual Studio 10.0\VC\vcvarsall.bat" x86
cd %~dp0
dumpbin /EXPORTS /OUT:<File_name>.def <File_name>.dll
lib /def:<File_name>.def /machine:x86
cd %CURPATH%
```

[visual studio command prompt 실행하기](https://stackoverflow.com/questions/5879076/how-to-create-a-batch-file-for-visual-studio-command-prompt)  
[bat 파일 현재 작업경로 얻기](https://devnote.tistory.com/154)  
[bat 파일의 경로 얻기](https://sunhyeon.wordpress.com/2012/08/05/161/)  
[dll 파일로 def 파일 만들기](https://igotit.tistory.com/entry/dll-%ED%8C%8C%EC%9D%BC%EB%A1%9C-lib-%EB%A7%8C%EB%93%A4%EA%B8%B0)  
[def 파일로 lib 파일 만들기](https://psychoria.tistory.com/221)
