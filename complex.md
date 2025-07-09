```

taskmaster/

├── app/                            # Asosiy modul (UI va navigatsiya)

│   ├── src/main/

│   │   ├── AndroidManifest.xml

│   │   └── kotlin/

│   │       └── MainActivity.kt

├── core/

│   ├── common/                     # Umumiy yordamchi sinflar

│   │   ├── src/main/kotlin/

│   │   │   ├── NetworkHelper.kt

│   │   │   ├── Result.kt

│   │   │   ├── DateFormatter.kt

│   │   │   └── Validators.kt

│   ├── ui/                         # Umumiy UI komponentlari

│   │   ├── src/main/kotlin/

│   │   │   └── components/

│   │   │       ├── CustomButton.kt

│   │   │       ├── LoadingBar.kt

│   │   │       ├── ErrorDialog.kt

│   │   │       └── ShimmerLoader.kt

│   ├── data/                       # Umumiy ma’lumotlar qatlami

│   │   ├── src/main/kotlin/

│   │   │   ├── api/

│   │   │   │   └── BaseApi.kt

│   │   │   ├── local/

│   │   │   │   ├── dao/UserDao.kt

│   │   │   │   ├── entity/UserEntity.kt

│   │   │   │   └── database/AppDatabase.kt

│   │   │   ├── repository/

│   │   │   │   └── UserRepositoryImpl.kt

│   │   │   └── mapper/

│   │   │       └── UserMapper.kt

│   ├── domain/                     # Umumiy biznes logikasi

│   │   ├── src/main/kotlin/

│   │   │   ├── model/

│   │   │   │   └── User.kt

│   │   │   ├── repository/

│   │   │   │   └── UserRepository.kt

│   │   │   └── usecase/

│   │   │       └── GetUserUseCase.kt

│   ├── designsystem/               # Dizayn tizimi

│   │   ├── src/main/kotlin/

│   │   │   ├── AppTheme.kt

│   │   │   ├── Colors.kt

│   │   │   ├── Typography.kt

│   │   │   └── Shapes.kt

├── features/

│   ├── auth/                       # Autentifikatsiya moduli

│   │   ├── src/main/kotlin/

│   │   │   ├── data/

│   │   │   │   ├── api/

│   │   │   │   │   └── AuthApi.kt

│   │   │   │   ├── local/

│   │   │   │   │   ├── dao/AuthDao.kt

│   │   │   │   │   └── entity/AuthEntity.kt

│   │   │   │   ├── repository/

│   │   │   │   │   └── AuthRepositoryImpl.kt

│   │   │   │   └── mapper/

│   │   │   │       └── AuthMapper.kt

│   │   │   ├── domain/

│   │   │   │   ├── model/

│   │   │   │   │   └── Auth.kt

│   │   │   │   ├── repository/

│   │   │   │   │   └── AuthRepository.kt

│   │   │   │   └── usecase/

│   │   │   │       ├── LoginUseCase.kt

│   │   │   │       ├── RegisterUseCase.kt

│   │   │   │       └── LogoutUseCase.kt

│   │   │   ├── presentation/

│   │   │   │   ├── screen/

│   │   │   │   │   ├── LoginScreen.kt

│   │   │   │   │   └── RegisterScreen.kt

│   │   │   │   ├── viewmodel/

│   │   │   │   │   └── AuthViewModel.kt

│   │   │   │   ├── state/

│   │   │   │   │   └── AuthState.kt

│   │   │   └── navigation/

│   │   │       └── AuthNavGraph.kt

│   ├── home/                       # Vazifalar ro‘yxati moduli

│   │   ├── src/main/kotlin/

│   │   │   ├── data/

│   │   │   │   ├── api/

│   │   │   │   │   └── TaskApi.kt

│   │   │   │   ├── local/

│   │   │   │   │   ├── dao/TaskDao.kt

│   │   │   │   │   └── entity/TaskEntity.kt

│   │   │   │   ├── repository/

│   │   │   │   │   └── TaskRepositoryImpl.kt

│   │   │   │   └── mapper/

│   │   │   │       └── TaskMapper.kt

│   │   │   ├── domain/

│   │   │   │   ├── model/

│   │   │   │   │   └── Task.kt

│   │   │   │   ├── repository/

│   │   │   │   │   └── TaskRepository.kt

│   │   │   │   └── usecase/

│   │   │   │       ├── GetTasksUseCase.kt

│   │   │   │       ├── AddTaskUseCase.kt

│   │   │   │       ├── DeleteTaskUseCase.kt

│   │   │   │       └── SyncTasksUseCase.kt

│   │   │   ├── presentation/

│   │   │   │   ├── screen/

│   │   │   │   │   └── TaskListScreen.kt

│   │   │   │   ├── viewmodel/

│   │   │   │   │   └── TaskViewModel.kt

│   │   │   │   ├── state/

│   │   │   │   │   └── TaskState.kt

│   │   │   └── navigation/

│   │   │       └── TaskNavGraph.kt

│   ├── test/                       # Test moduli

│   │   ├── src/main/kotlin/

│   │   │   ├── data/

│   │   │   │   ├── api/

│   │   │   │   │   └── TestApi.kt

│   │   │   │   ├── local/

│   │   │   │   │   ├── dao/TestDao.kt

│   │   │   │   │   └── entity/TestEntity.kt

│   │   │   │   ├── repository/

│   │   │   │   │   └── TestRepositoryImpl.kt

│   │   │   │   └── mapper/

│   │   │   │       └── TestMapper.kt

│   │   │   ├── domain/

│   │   │   │   ├── model/

│   │   │   │   │   └── TestQuestion.kt

│   │   │   │   ├── repository/

│   │   │   │   │   └── TestRepository.kt

│   │   │   │   └── usecase/

│   │   │   │       ├── GetTestQuestionsUseCase.kt

│   │   │   │       └── SubmitTestUseCase.kt

│   │   │   ├── presentation/

│   │   │   │   ├── screen/

│   │   │   │   │   └── TestScreen.kt

│   │   │   │   ├── viewmodel/

│   │   │   │   │   └── TestViewModel.kt

│   │   │   │   ├── state/

│   │   │   │   │   └── TestState.kt

│   │   │   └── navigation/

│   │   │       └── TestNavGraph.kt

│   ├── profile/                    # Profil moduli

│   │   ├── src/main/kotlin/

│   │   │   ├── data/

│   │   │   │   ├── api/

│   │   │   │   │   └── ProfileApi.kt

│   │   │   │   ├── local/

│   │   │   │   │   ├── dao/ProfileDao.kt

│   │   │   │   │   └── entity/ProfileEntity.kt

│   │   │   │   ├── repository/

│   │   │   │   │   └── ProfileRepositoryImpl.kt

│   │   │   │   └── mapper/

│   │   │   │       └── ProfileMapper.kt

│   │   │   ├── domain/

│   │   │   │   ├── model/

│   │   │   │   │   └── Profile.kt

│   │   │   │   ├── repository/

│   │   │   │   │   └── ProfileRepository.kt

│   │   │   │   └── usecase/

│   │   │   │       ├── GetProfileUseCase.kt

│   │   │   │       └── UpdateProfileUseCase.kt

│   │   │   ├── presentation/

│   │   │   │   ├── screen/

│   │   │   │   │   └── ProfileScreen.kt

│   │   │   │   ├── viewmodel/

│   │   │   │   │   └── ProfileViewModel.kt

│   │   │   │   ├── state/

│   │   │   │   │   └── ProfileState.kt

│   │   │   └── navigation/

│   │   │       └── ProfileNavGraph.kt

├── di/                             # Hilt modullari

│   ├── src/main/kotlin/

│   │   ├── AppModule.kt

│   │   ├── NetworkModule.kt

│   │   ├── DatabaseModule.kt

│   │   └── RepositoryModule.kt

└── logic/                          # Murakkab logika

&nbsp;   ├── src/main/kotlin/

&nbsp;   │   ├── TestLogic.kt

&nbsp;   │   └── StatsLogic.kt

```

