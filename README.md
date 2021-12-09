# react-native-boilerplate
명령어 모음 
### React Native Preference Setting

1. Navigation Set up

```
yarn add @react-navigation/bottom-tabs @react-navigation/native @react-navigation/native-stack @react-navigation/stack
```

2. StyledComponentes Set up

```
yarn add @types/styled-components @types/styled-components-react-native
```

### 마무리.
```
npx pod-install ios
```

# firebase 사용관련

## 안드로이드 세팅

### Android firebase setup 후 빌드 오류날시

1. [패키지명]/android/app/src/main/assets 폴더가 있는지 확인하고 없으면 생성

2. [패키지명]/android 폴더에서 ./gradlew clean 실행

3. [패키지명] 폴더에서 아래 명령어 실행

```
react-native bundle --platform android --dev false --entry-file index.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res
```

4. react-native run-android
