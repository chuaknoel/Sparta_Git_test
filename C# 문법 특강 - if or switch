# C# 문법 특강 - if / switch

## if문
### 개요
- 프로그래밍에서 가장 많이 사용되는 제어문 중 하나입니다.
- 조건문을 사용하여 특정 조건에 따라 코드 블록을 실행하는 제어문입니다.
- 조건식이 true일 경우에만 실행됩니다.

### if 문 기본
#### 문법
```csharp
if (조건식)
{
    // 조건식이 참일 때 실행되는 구문
}
```

#### BSD 스타일 (Allman 스타일)
```csharp
if (조건식)
{
    // 조건식이 참일 때 실행되는 구문
}
else
{
    // 조건식이 거짓일 때 실행되는 구문
}
```
#### K&R 스타일 (Inline 스타일)
```csharp
if (조건식) {
    // 조건식이 참일 때 실행되는 구문
} else {
    // 조건식이 거짓일 때 실행되는 구문
}
```

#### 예제

```csharp
// Boolean 타입 - true 또는 false 값만 가질 수 있다.
bool isGameOver = false;

if (isGameOver)
{
    // 게임이 종료된 경우
    Console.WriteLine("게임이 종료되었습니다.");
}
```

```csharp
bool hasKey = false;

// 중괄호 {} 없는 if문 (한 줄만 실행할 경우)
if (hasKey == true)
    Console.WriteLine("열쇠를 가지고 있습니다."); // 한 줄만 if문에 포함됨
```

```csharp
bool isPlayerDead = false;

if (isPlayerDead == false)
{
    Console.WriteLine("플레이어가 살아있습니다.");
}

if (!isPlayerDead)
{
    Console.WriteLine("플레이어가 살아있습니다.");
}
```

### if-else 문
#### 문법
```csharp
if (조건식)
{
    // 조건식이 참일 때 실행되는 구문
}
else
{
    // 조건식이 거짓일 때 실행되는 구문
}
```

#### 예제

```csharp
bool isGameOver = false;

if (isGameOver)
{
    // 게임이 종료된 경우
    Console.WriteLine("게임이 종료되었습니다.");
}
else
{
    // 게임이 종료되지 않은 경우
    Console.WriteLine("게임이 진행 중입니다.");
}
```

```csharp
bool hasKey = false;

// 중괄호 {} 없는 if-else문 (한 줄만 실행할 경우)
if (hasKey)
    Console.WriteLine("열쇠를 가지고 있습니다."); // 한 줄만 if문에 포함됨
else
    Console.WriteLine("열쇠가 없습니다."); // 한 줄만 else문에 포함됨
```

### if-else if-else 문
#### 문법
```csharp
if (조건식1)
{
    // 조건식1이 참일 때 실행되는 구문
}
else if (조건식2)
{
    // 조건식2가 참일 때 실행되는 구문
}
else
{
    // 모든 조건식이 거짓일 때 실행되는 구문
}
```

#### 예제

```csharp
int playerLevel = 5;

if (playerLevel < 10)
{
    Console.WriteLine("쪼렙");
}
else if (playerLevel < 20)
{
    Console.WriteLine("중수");
}
else
{
    Console.WriteLine("고인물");
}  
```

### 연산자

#### 비교 연산자

- == (같다) : 두 값이 같을 때 true
- &gt; (크다) : 왼쪽 값이 오른쪽 값보다 클 때 true
- < (작다) : 왼쪽 값이 오른쪽 값보다 작을 때 true
- &gt;= (크거나 같다) : 왼쪽 값이 오른쪽 값보다 크거나 같을 때 true
- <= (작거나 같다) : 왼쪽 값이 오른쪽 값보다 작거나 같을 때 true
- != (같지 않다) : 두 값이 다를 때 true
    
#### 논리 연산자
- && (AND) : 두 조건이 모두 true일 때 true
- || (OR) : 두 조건 중 하나라도 true일 때 true
- ! (NOT) : 조건이 false일 때 true

#### 삼항 연산자

- if-else 문을 간단하게 표현하는 문법
  
```
변수 = (조건식) ? 참일 때 값 : 거짓일 때 값
```

- 단순한 삼항 연산자의 경우 코드의 가독성이 높아지고, 간결하게 표현
- 하지만 복잡한 조건문을 사용할 경우 가독성이 떨어질 수 있습니다.

```csharp
int playerHealth = 30;
string msg;

// 삼항 연산자 기본 구조: (조건) ? 참일 때 값 : 거짓일 때 값
msg = (playerHealth > 0) ? "플레이어 생존" : "게임 오버";
Console.WriteLine(msg);
```

```csharp
// if-else 대신 삼항 연산자 사용
int score = 95;
string grade = (score >= 90) ? "A" : "B";
Console.WriteLine($"점수: {score}, 등급: {grade}");
```

## switch문
### 개요
- switch문은 여러 조건을 비교하여 해당하는 코드 블록을 실행하는 제어문

#### 문법
```csharp
switch (변수)
{
    case 값1:
        // 값1과 일치할 때 실행되는 구문
        break;
    case 값2:
        // 값2와 일치할 때 실행되는 구문
        break;
    default:
        // 모든 case와 일치하지 않을 때 실행되는 구문
        break;
}
```
#### 예제
```csharp
int weaponId = 2;
string weaponName;

switch (weaponId)
{
    case 1:
        weaponName = "검";
        break;
        
    case 2:
        weaponName = "활";
        break;
        
    case 3:
        weaponName = "도끼";
        break;
        
    case 4:
        weaponName = "창";
        break;
        
    default:
        weaponName = "주먹";
        break;
}

Console.WriteLine($"현재 무기: {weaponName}");
```

#### 예제 2 - case grouping

```csharp
char buttonPressed = 'A';
string action;

switch (buttonPressed)
{
    case 'W':
    case 'w':
        action = "앞으로 이동";
        break;
        
    case 'A':
    case 'a':
        action = "왼쪽으로 이동";
        break;
        
    case 'S':
    case 's':
        action = "뒤로 이동";
        break;
        
    case 'D':
    case 'd':
        action = "오른쪽으로 이동";
        break;
        
    case 'J':
    case 'j':
    case ' ':  // 스페이스바
        action = "점프";
        break;
        
    default:
        action = "아무 동작 없음";
        break;
}

Console.WriteLine($"입력 버튼: {buttonPressed}, 수행 동작: {action}");
```
