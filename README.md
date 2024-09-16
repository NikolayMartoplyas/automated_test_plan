# **План автоматизации тестирования _записи на обучение профессии «Инженер по тестированию»_**
------------------------------
### 1. [Перечень автоматизированных сценариев](#перечень-автоматизированных-сценариев)
### 2. [Перечень используемых инструментов с обоснованием выбора](#перечень-используемых-инструментов-с-обоснованием-выбора)
### 3. [Перечень необходимых разрешений, данных и доступов](#перечень-необходимых-разрешений,-данных-и-доступов)
### 4. [Перечень и описание возможных рисков при автоматизации](#перечень-и-описание-возможных-рисков-при-автоматизации)
### 5. [Перечень необходимых специалистов для автоматизации](#перечень-необходимых-специалистов-для-автоматизации)
### 6. [Интервальная оценка с учётом рисков в часах](#интервальная-оценка-с-учётом-рисков-в-часах)

-------------------------------

## 1. Перечень автоматизированных сценариев <a name="перечень-автоматизированных-сценариев"></a>

1. [Переход к форме записи №1](#переход-к-форме-записи-№1)
2. [Переход к форме записи №2](#переход-к-форме-записи-№2)
3. [Заполнение формы и отправка формы валидными данными](#заполнение-формы-и-отправка-формы-валидными-данными)
4. [Заполнение и отправка формы не валидными данными](#заполнение-и-отправка-формы-не-валидными-данными)

### 1.Переход к форме записи №1 <a name="Переход-к-форме-записи-№1"></a>
#### Шаги

1. Открыть сайт [netology.ru](https://netology.ru/)
2. В верху сайта найти поисковую строку **каталог курсов** и нажать на нее
3. В открывшемся списке найти  **программирование**
5. В поисковой строке ввести **Инженер по тестированию**
6. В открывшемся списке выбрать курс **Инженер по тестированию**
7. На открывшейся страницу проскролить в низ до записи на курс
8.
![image](https://github.com/user-attachments/assets/75da5791-1f2b-49e2-a449-f4be26883a60)

### **Ожидаемый результат:** попасть на страницу записи на курс 

### 2. Переход к форме записи №2 <a name="переход-к-форме-записи-№2"></a>

1.  Открыть сайт [netology.ru](https://netology.ru/)
2. Проскролить страницу в низ и найти раздел направление обучения 
3. 
![image](https://github.com/user-attachments/assets/560eded3-a47b-47fe-bdbf-9c35ee106f88)

4. Выбрать направление программирование
5. На открывшейся странице в списке найти раздел **Инженер по тестированию**
6. 
![image](https://github.com/user-attachments/assets/0f849ecd-95c9-404e-9682-f5ec94b85ce2)
7. На открывшейся странице проскролить в низ до записи на курс
8. 
![image](https://github.com/user-attachments/assets/e6b790a6-9067-4e95-80d9-c364ccd9bb44)

**Ожидаемый результат:** попасть на страницу записи на курс

### 3. Заполнение формы и отправка формы валидными данными <a name="заполнение-формы-и-отправка-формы-валидными-данными"></a>

1. В поле **имя** ввести значения например **Виктор**
2. В поле **номер телефона** ввести значения например **+7 988 999 99 99**
3. В поле **электронная почта** ввести значения например **incognito@mail.ru** 
4. Нажать кнопку записаться

**Ожидаемый результат:** запись отправлена, появляется сообщение что запись на курс "инженер по тестированию" успешно оформлена, с вами свяжется специалист для дальнейшего координирования

### 4. Заполнение и отправка формы не валидными данными <a name="заполнение-и-отправка-формы-не-валидными-данными"></a>
#### _Кейс №1_
1. Поле **имя** оставить пустым
2. В поле **номер телефона** ввести значения например **+7 988 999 99 99**
3. В поле **электронная почта** ввести значения например **incognito@mail.ru** 
4. Нажать кнопку записаться

**Ожидаемый результат**: форма не отправлена, поле имя подсвечивается красным, подпись в низу **Обязательное поле**

![image](https://github.com/user-attachments/assets/5216ab72-cda7-410b-bc67-fd822a19f93b)

#### _Кейс №2_

1. Поле **имя** ввести спецсимволы
2. В поле **номер телефона** ввести значения например **+7 988 999 99 99**
3. В поле **электронная почта** ввести значения например **incognito@mail.ru** 
4. Нажать кнопку записаться

**Ожидаемый результат**: форма не отправлена, поле имя подсвечивается красным, подпись в низу **Должно состоять из букв**

![image](https://github.com/user-attachments/assets/d9606d9e-1001-4059-87f8-0a1776f65a49)

#### _Кейс №3_

1. Поле **имя** ввести значения например **Виктор**
2. В поле **номер телефона** оставить поле пустым
3. В поле **электронная почта** ввести значения например **incognito@mail.ru** 
4. Нажать кнопку записаться

**Ожидаемый результат:** форма не отправлена, поле телефон подсвечивается красным, подпись в низу **Обязательное поле**

![image](https://github.com/user-attachments/assets/ee0b0590-ffae-4390-b562-f10e8cbc01d1)

#### _Кейс №4_

1. Поле **имя** ввести значения например **Виктор**
2. В поле **номер телефона** ввести буквы
3. В поле **электронная почта** ввести значения например **incognito@mail.ru** 
4. Нажать кнопку записаться

**Ожидаемый результат:** форма не отправлена, поле телефон подсвечивается красным, подпись в низу **Неверный формат**

![image](https://github.com/user-attachments/assets/1f18d1e4-97c2-4850-9860-8946dbf568a5)

#### _Кейс №5_

1. Поле **имя** ввести значения например **Виктор**
2. В поле **номер телефона** ввести значения например **+7 988 999 99 99**
3. В поле **электронная почта** оставить поле пустым
4. Нажать кнопку записаться

**Ожидаемый результат:** форма не отправлена, поле электронная почта подсвечивается красным, подпись в низу **Обязательное поле**

![image](https://github.com/user-attachments/assets/3b24213a-139d-4091-a359-42fea3064d0d)

#### _Кейс №6_

1. Поле **имя** ввести значения например **Виктор**
2. В поле **номер телефона** ввести значения например **+7 988 999 99 99**
3. В поле **электронная почта** ввести значения например **incognito@mail** без домена 
4. Нажать кнопку записаться

**Ожидаемый результат:** форма не отправлена, поле электронная почта подсвечивается красным, подпись в низу **Неверный email**

![image](https://github.com/user-attachments/assets/7e72277f-8fb0-4827-8896-7b03fc2c83d9)

-------------------

## 2. Перечень используемых инструментов с обоснованием выбора <a name="перечень-используемых-инструментов-с-обоснованием-выбора"></a>

### _Selenide_
- Обеспечивает простоту использования благодаря лаконичному и интуитивно понятному API, сам код получается не растянутым.
- поддерживает работу с различными браузерами (Chrome, Firefox, Safari и т.д.)
- имеет хорошие интеграции с популярными фреймворками тестирования, такими как JUnit

### _JUnit5_
- Используется для написания тестов и организации их выполнения

### _Gradle_
- Для управления зависимостями и сборки проектов.

### _Allure Report_
- Для сборки и анализа отчетов о проведении тестов.
------------------------------

### 3. Перечень необходимых разрешений, данных и доступов <a name="перечень-необходимых-разрешений,-данных-и-доступов"></a>

- Доступ к тестовому режиму
- Тестовые данные
- Разрешение на тестирование сайта

________________

### 4. Перечень и описание возможных рисков при автоматизации <a name="перечень-и-описание-возможных-рисков-при-автоматизации"></a>

- Непредвиденные изменения в интерфейсе пользователя, которые могут сломать существующие тесты.
- Возможные проблемы с производительностью при больших объемах данных.
- Ошибки при взаимодействии с внешними системами.
- Непрерывный доступ к тестовым средам.
- Ошибки на сервере

___________________

### 5. Перечень необходимых специалистов для автоматизации <a name="перечень-необходимых-специалистов-для-автоматизации"></a>

- Автоматизированный тестировщик

____________________

### 6. Интервальная оценка с учётом рисков в часах <a name="интервальная-оценка-с-учётом-рисков-в-часах"></a>

- Написание кода для автоматизированных сценариев и кейсов - 8 часов
- Подготовка отчетности и документации - 4 часа
- Запас времени на непредвиденные сценарии - 3 часа
- ВСЕГО - 15 часов







