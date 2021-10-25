# Настройка Git и GitHub в Intellij IDEA

## 1. Добавить аккаунт GitHub в Intellij IDEA

### 1.1 Создать access token

![Personal access token page](./pictures/GitHub_Token.png "Token")

*Перейди в настройки GitHub -> Developer Settings -> Personal access token
-> Generate new token*

![Token generation page](./pictures/Allowed.png "Required scopes")

Оставьте только scope'ы: repo, workflow, read:org и gist.

Появится токен. **Обязательно скопируйте его, потому что после того, как вы закроете страницу, он пропадёт!**

### 1.2 Добавить аккаунт в Intellij IDEA

Зайдите в Intellij IDEA. Там File->Settings->Version Control->GitHub.

![Settings page in IDEA for GitHub](./pictures/Settings_Intellij_IDEA.png "IDEA GitHub Account")

Там уже нажмите *Ctrl+N(на Mac Cmd+N)->Login with token*. И просто вставьте ваш скопированный токен в поле.
Add account. *Поздравляю, вы добавили GitHub аккаунт!*

---
## 2. Применение

### 2.1 Скачать проект с GitHub

Для того чтобы клонировать проект, достаточно зайти в *File->New->Project from Version Control*.

![Clone project from GitHub](./pictures/GitHub_clone_proj.png "Clone project")

Теперь достаточно выбрать проект и нажать *Clone*.

### 2.2 Сделать Commit

Достаточно нажать *Git->Commit*. Откроется вкладка *Commit*.

![Tab for committing to git](./pictures/Commit_tab.png "Commit tab in IDEA")

В *Unversioned Files* находятся файлы не добавленные в *staging area*. Там можно их добавить, чтобы они попали в следующий коммит.
В *Changes* можно убрать файлы, которые не должны попасть в следующий коммит.

Когда файлы выбранный, можно написать сообщение для коммита и сделать его, нажав кнопку *Commit*.

### 2.3 Сделать Push

Это можно сделать из той же вкладки, нажав *Commit and Push*, после чего файлы загрузятся на удалённый репозиторий.

Так же это можно сделать перейдя *Git->Push*