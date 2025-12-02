# Инструкция по публикации на GitHub и настройке GitHub Pages

## Шаг 1: Создание репозитория на GitHub

1. Перейдите на https://github.com/new
2. Заполните:
   - **Repository name**: `payment-form` (или другое название)
   - **Description**: Отраслевая платежная форма
   - **Visibility**: Public или Private (на ваш выбор)
   - **НЕ** добавляйте README, .gitignore или лицензию (они уже есть)
3. Нажмите "Create repository"

## Шаг 2: Подключение локального репозитория к GitHub

После создания репозитория GitHub покажет инструкции. Выполните команды (замените `YOUR_USERNAME` на ваш GitHub username):

```bash
cd "/Users/m.apalishin/Desktop/⚒️ Отраслевая платежная форма_v1"
git remote add origin https://github.com/YOUR_USERNAME/payment-form.git
git branch -M main
git push -u origin main
```

## Шаг 3: Настройка GitHub Pages

1. Перейдите в настройки репозитория: `Settings` → `Pages`
2. В разделе "Source" выберите:
   - **Branch**: `main`
   - **Folder**: `/ (root)`
3. Нажмите "Save"

GitHub Pages будет доступен по адресу:
`https://YOUR_USERNAME.github.io/payment-form/`

## Альтернативный способ через GitHub CLI

Если у вас установлен GitHub CLI, можно выполнить:

```bash
gh repo create payment-form --public --source=. --remote=origin --push
```

Затем настроить Pages через веб-интерфейс (шаг 3 выше).

