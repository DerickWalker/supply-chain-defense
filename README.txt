공급망 공격 교육용 게임 "supply-chain-defense"

공급망 해킹 공격에 대해서 공부할수있게 게임으로 해볼수있는 프로그램을 가져왔습니다
해당 프로그램은 실제 사례와 기법을 기반으로 교육 목적을 위해 개발되었습니다
아쉽게도 업로드 가능한 용량 이슈로 exe파일은 올리지 못했습니다
설치없이 HTML 파일을 다운 받으신후 크롬 브라우저로 여신후 사용도 가능합니다
단순한 방식이긴 하지만 실제 피해가 많은 공격 기법으로서 이를 대비하기 위해 어떻게 하는것이고 해커는 어떻게 공격을 시도하는건지 원리를 이해하시고 공부해가시기 바랍니다
'일반인' 난이도는 턴제 방식처럼 단순히 딸깍 하는 수준으로 상당히 쉬운 정도로 만들었지만,
'전문가' 난이도는 턴제가 아닌 실시간으로 탐지및 침투 공격등이 들어오는걸 방어하며 실제 코드를 입력하도록 하였습니다
다들 즐겁게 해보시고 버그나 수정할 점이 있으시다면 언제든 알려주세요
그럼 감사합니다

Supply Chain Defense — Usage Guide
====================================

[supply-chain-defense.html]
Open it in any browser to play immediately. No installation needed.

[mobile-install folder]
To install this on mobile as an app (PWA), the folder needs to be hosted
on the web first:
1. Drag and drop this folder onto vercel.com/new (or run `npx vercel --prod`
   from inside it)
2. Open the resulting https link on your phone's browser
3. You'll be prompted to "Add to Home Screen" / "Install app" — do that
Opening index.html directly (locally) still runs the game fine, but the
install prompt itself only shows up once it's served over https.

[desktop-source folder]
Source for the Windows/Mac/Linux desktop app. A pre-built .exe isn't
included in this download to keep the file size small — Electron apps
bundle a full browser engine, so the compiled app is always ~70MB
regardless of how simple the game itself is, and compressing it further
doesn't help (it's already compressed internally).

To build it yourself, it only takes two commands. From inside this folder,
with Node.js installed:
  npm install
  npm run dist:win    (produces a Windows .exe in a new "dist" folder)
  npm run dist:mac    (Mac)
  npm run dist:linux  (Linux)

If you'd rather not build it yourself, ask and a pre-built .exe can be
provided as its own separate download instead.
