  # Инструкция для VSCode для использования Copilot агентов.

  В настройках VSCode поставить галочку
  ![image](https://github.com/user-attachments/assets/e153c9c2-2a47-4d71-875b-5e7fc5e6923b)


1. Создать файл по пути: ```{your_project}\.github\copilot-instructions.md```
2. В файле написать инструкции для агента, по примеру в репозитории

Как использовать отписание проекта, еще не понял.

Справка: https://code.visualstudio.com/docs/copilot/copilot-customization

## Шаблон для новых проектов

1. Установить расширение (Extension) - Project Templates
2. Ввести команду: ```>Save Project as Template```
   
   ![image](https://github.com/user-attachments/assets/ccaaa9d5-2f84-49f1-b646-0aee8de9aa4e)

4. Задать имя шаблону. Например ```Copilot Agent```
5. Папку с шаблоном можно открыть в проводнике и отредактировать
   
  ![image](https://github.com/user-attachments/assets/b309a5e0-009f-4811-b6a3-b54ae2b49b63)

6. Project Templates сохраняет шаблоны в: ```C:\Users\{USER_NAME}\AppData\Roaming\Code\User\ProjectTemplates```
7. Для использования шаблона ( добавить в текущий проект):
   * в EXPLORER (окно проекта) нажать в свободной области правую кнопку мыши - ``` Create Project from Template```
   * выбрать имя шаблона
  
  ![image](https://github.com/user-attachments/assets/8e62ca4b-bc5e-4877-9077-9e41708112eb)


# Различия трех версий

Ниже приведено сравнение трех версий системных промтов с разными подходами к обеспечению наивысшего качества кода в условиях enterprise-проектов.

---

## 1. Подход к решению задачи и планирование

### Первый промт
- Содержит подробные пошаговые инструкции, ориентированные на строгое соблюдение стандартов.
- Фокусируется на конкретных аспектах: тестирование, логирование, обновление README.
- Не уделяет явного внимания предварительному планированию.

### Второй промт
- Предоставляет сжатый набор правил, охватывающих основные принципы (PEP8, архитектура, тестирование).
- Не детализирует процесс планирования и уточнения требований.

### Третий промт
- Акцентирует внимание на тщательном анализе запроса перед внесением изменений.
- Включает шаги по разработке краткого плана или псевдокода.
- Предусматривает уточнение неясных требований посредством вопросов.
- Такой подход способствует более осмысленным, обоснованным изменениям.

---

## 2. Фокус на минимальных и целенаправленных изменениях

### Первый промт
- Детально прописывает ограничения по изменению кода.
- Требует, чтобы изменения были минимальными и точными, без радикальных переписываний.
- Ограничения распространяются также на архитектуру проекта.

### Второй промт
- Содержит аналогичные рекомендации, но в более сжатой форме, без излишних деталей.

### Третий промт
- Подчеркивает принцип минимальности: только изменения, необходимые для решения задачи.
- Предотвращает создание лишних файлов или функций.
- Способствует сохранению чистоты кода, что особенно важно в условиях enterprise-проектов.

---

## 3. Соблюдение стандартов и документация

### Первый промт
- Очень детально охватывает аспекты кода: от PEP8 и именования до использования докстрингов, комментариев, тестирования и обновления README.
- Особое внимание уделяется управлению зависимостями и архитектурным аспектам (структура папок, логическая группировка).

### Второй промт
- Затрагивает те же аспекты, но в более лаконичном виде.
- Может упустить некоторые важные нюансы для глубокого контроля качества кода.

### Третий промт
- Требует соблюдения PEP8, использования типизации, докстрингов и комментариев.
- Делает акцент на чистоту, модульность и соответствие лучшим практикам.
- Не вдается в подробности по управлению зависимостями или тестовой инфраструктурой, что может быть как плюсом (простота), так и минусом (менее детальный контроль).

---

## 4. Взаимодействие с пользователем и профессиональный тон

### Первый промт
- Включает инструкции по уточнению запросов.
- Требует подтверждения каждого изменения.
- Обеспечивает высокую точность, но может замедлять процесс при частых итерациях.

### Второй промт
- Менее детализирован в части взаимодействия.
- Может быть проще в использовании, но потенциально менее адаптивен при сложных запросах.

### Третий промт
- Явно предписывает анализировать запрос, задавать уточняющие вопросы и разрабатывать план перед внесением изменений.
- Ориентирован на лаконичные объяснения и предоставление кода в виде коротких диффов.
- Обеспечивает профессиональную коммуникацию и повышает доверие к вносимым изменениям.

---

## 5. Итоговое сравнение

- **Первый промт**  
  Наиболее подробный и жестко регламентированный. Подходит для ситуаций, где требуется максимальное соблюдение стандартов (например, в крупных корпоративных проектах с жестким контролем качества).

- **Второй промт**  
  Предлагает краткий и сжатый набор правил, который охватывает основные моменты. Однако может упустить некоторые детали, необходимые для глубокого контроля над качеством кода.

- **Третий промт**  
  Балансирует между детализацией и лаконичностью. Делает упор на предварительный анализ, планирование и минимальные, целенаправленные изменения. Такой подход обеспечивает высокую точность и обоснованность изменений, что особенно важно при адаптивном и профессиональном взаимодействии.

---

**Вывод:**  
Для обеспечения наивысшего качества кода в условиях enterprise-проектов третий промт оказывается наиболее эффективным. Он сочетает строгие стандарты с гибким подходом к анализу и планированию изменений, способствуя созданию чистого, поддерживаемого и качественного кода.

