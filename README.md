# 프로젝트 설정 가이드

이 문서는 Gemini CLI 및 Git을 포함한 개발 환경 설정에 대한 지침을 제공합니다.

## 1. Gemini CLI 전역 설정 (Windows)

다음 단계는 Windows 시스템에 Gemini CLI를 설치하고 구성하는 과정을 안내합니다.

### 전제 조건

-   **Node.js 및 npm:** Gemini CLI는 Node.js (버전 20 이상)를 필요로 합니다. npm은 Node.js 설치에 포함되어 있습니다.

### 설치

1.  **Node.js 설치:**
    Node.js는 공식 웹사이트에서 다운로드하여 설치하거나 Winget과 같은 패키지 관리자를 사용할 수 있습니다. 관리자 권한으로 PowerShell을 열고 다음을 실행합니다:
    ```powershell
    winget install OpenJS.NodeJS.LTS --silent
    ```

2.  **Gemini CLI 설치:**
    Node.js 설치가 완료되면, 관리자 권한으로 새 PowerShell 또는 명령 프롬프트 창을 열고 다음 명령어를 실행하여 Gemini CLI를 전역으로 설치합니다:
    ```powershell
    npm install -g @google/gemini-cli
    ```

### 첫 번째 구성

1.  **로그인:**
    설치가 완료되면 새 터미널 창에서 `gemini` 명령어를 실행합니다:
    ```powershell
    gemini
    ```

2.  **인증:**
    CLI는 첫 번째 설정을 안내할 것입니다. CLI를 인증하기 위해 Google 계정으로 로그인하라는 메시지가 표시됩니다.

## 2. Git 구성

Git 계정을 연결하려면 사용자 이름과 이메일을 구성해야 합니다. 이 정보는 커밋을 식별하는 데 사용됩니다.

1.  **이메일 설정:**
    터미널을 열고 다음 명령어를 실행하여 이메일을 자신의 이메일로 교체합니다.
    ```bash
    git config --global user.email "h.yeon030728@gmail.com"
    ```

2.  **사용자 이름 설정:**
    다음으로 사용자 이름을 설정합니다.
    ```bash
    git config --global user.name "Your-Username"
    ```
    * "Your-Username"을 원하는 Git 사용자 이름으로 교체하세요.

3.  **구성 확인:**
    다음 명령어로 구성이 올바르게 설정되었는지 확인할 수 있습니다:
    ```bash
    git config --global user.email
    git config --global user.name
    ```