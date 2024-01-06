# Commit message

GC Project Space의 컨밴션은 아래의 레퍼런스를 따릅니다.

- [Gitmoji](https://gitmoji.dev/)
- [Udacity Git Commit Message Style Guide](https://udacity.github.io/git-styleguide/)
- [Github Commit Message Rules](https://junhyunny.github.io/information/github/git-commit-message-rule/)

## 1. Importance of Commit Message

> 커밋 메세지를 작성할 때 규칙이 필요한 이유는 다음과 같습니다.

- 팀원과의 원활한 소통을 위해
- 편리한 history 추적을 위해
- 이슈(issue) 관리를 위해

## 2. Commit message format

> 커밋 메세지의 기본 포멧은 아래의 명세를 따릅니다.

```git
:Emoji: <type>: <subject>

<body>

<footer>
```

### 2.1 Type & Emoji

> 해당 커밋은 무엇에 대한 작업인지 키워드를 통해 표시합니다.

| Emoji | Type | Description |
|:----:|:-----:|:-----------:|
| ✨(sparkles) | Feat | 새로운 기능 추가 |
| 🐛 (bug) | Fix | 버그 수정 |
| 📝 (memo) | Docs | 문서 수정 |
| 🎨 (art) | Style | 코드 포맷팅, 세미콜론 누락, 코드 변경이 없는 경우 |
| ♻️ (recycle) | Refactor | 코드 리팩토링 |
| ✅ (white_check_mark) | Test | 테스트 코드, 리팩토링 테스트 코드 추가 |
| 🔧 (wrench) | Chore | 빌드 업무 수정, 패키지 매니저 수정 |
| 🧪 (test_tube) | Test | test 관련 코드 수정 |

### 2.2 Subject

> 해당 커밋에 대한 간단한 한줄 요약 내용을 작성합니다.

- 50자를 넘기지 않고, 마침표 및 특수기호를 사용하지 않습니다.
- 영문으로 시작하는 경우 동사(원형)를 가장 앞에 두고 첫 글자는 대문자로 작성합니다. (과거시제 사용 금지)
- 제목은 개조식으로 작성합니다.

**Bad**

```git
:bug: Fix: 버그 수정
```

**Good**

```git
:bug: Fix: 로그인 API refresh token 오류 수정
```

### 2.3 Body (선택사항)

> 해당 커밋에 대한 상세 내용을 작성합니다.

- 선택 사항임으로 모든 커밋에 작성할 필요는 없습니다.
- 한 줄에 72자를 넘기지 않습니다.
- 어떻게(how)보다 무엇(what)과 왜(why)를 설명합니다.
- 작업 설명뿐만이 아니라 커밋의 이유를 작성할 때에도 사용합니다.

**Example**

```git
:sparkles: Feat: 게시글 작성 API 추가

게시글 작성 API를 추가
- PostController.java: 기능 추가로 인한 컨트롤러 수정
- PostService.java: 기능 추가로 인한 서비스 수정
- PostRepository.java: 기능 추가로 인한 레포지토리 수정
```

### 2.4 Footer (선택사항)

> 커밋 메세지의 맺음말입니다.

- 선택 사항이므로 모든 커밋에 작성할 필요는 없습니다.
- 이슈를 추적하기 위한 ID를 추가할 때 사용합니다.
  - 해결 - 해결한 이슈 ID
  - 관련 - 해당 커밋에 관련된 이슈 ID
  - 참고 - 참고할만한 이슈 ID

**Example of Footer**

```git
해결: #123
관련: #321
참고: #222
```

**Exmample of Full Commmit Message**

```git
:sparkles: Feat: 게시글 작성 API 추가 (#123)

게시글 작성 API를 추가
- PostController.java: 기능 추가로 인한 컨트롤러 수정
- PostService.java: 기능 추가로 인한 서비스 수정
- PostRepository.java: 기능 추가로 인한 레포지토리 수정

해결: #123
참고: #321
```
