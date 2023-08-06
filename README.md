# 🧩 Code_Snippet
> 코드 조각을 모아두기 위한 목적으로 생성된 레포토리입니다.

## 🔍 사용 방법
+ *.snippet 확장자의 파일을 작성합니다.
+ C# 기준으로 `C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\VC#\Snippets\1042` 하위 경로에 폴더를 생성하여 파일을 추가합니다.
+ Visual Studio에서 `도구 → 코드 조각 관리자` 탭을 열어서 `CSharp` 언어를 선택하고, 위에서 생성한 폴더를 추가합니다.
+ Visual Studio를 재시작합니다.
+ 단축키 `Ctrl + K, X`를 눌러 코드 조각을 불러옵니다.

## 📃 Snippet 양식
+ Debug.Log문을 생성하는 xml의 예시입니다.
```xml
<?xml version="1.0" encoding="utf-8"?>
<CodeSnippets xmlns="http://schemas.microsoft.com/VisualStudio/2005/CodeSnippet">
	<CodeSnippet Format="1.0.0">
		<Header>
			<Title>Debug</Title>
			<Shortcut>db</Shortcut>
			<Description>Debug.Log문을 만들어냅니다.</Description>
			<Author>gskim</Author>
			<SnippetTypes>
				<SnippetType>Expansion</SnippetType>
				<SnippetType>SurroundsWith</SnippetType>
			</SnippetTypes>
		</Header>
		<Snippet>
			<Declarations>
				<Literal>
					<ID>variable</ID>
					<Default>var</Default>
				</Literal>
			</Declarations>
			<Code Language="csharp"><![CDATA[Debug.Log($$"$variable$ : {$variable$}");$end$]]>
			</Code>
		</Snippet>
	</CodeSnippet>
</CodeSnippets>
```
