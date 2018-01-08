---
lang: ru
layout: article_with_sidebar
updated_at: '2018-01-08 11:55 +0400'
title: Настройка авторизации через Facebook
order: 20
published: false
identifier: ref_fblogin
---
Чтобы в магазине появилась кнопка **Войти через Facebook**, понадобится:

1.  Настроенное [приложение Facebook](#creating-a-facebook-app) 
2.  _Идентификатор приложения_ и _Секрет приложения_ для настройки модуля **Social Login** в X-Cart [Configuring the Social Login module: Facebook](#configuring-the-social-login-module-facebook)

## Как создать приложение в Facebook

1.  Авторизуйтесь в [Facebook для разработчиков](https://developers.facebook.com/apps).

2.  Нажмите **Создать приложение**:
    ![2.jpg]({{site.baseurl}}/attachments/ref_fblogin/2.jpg)

    Откроется окно **Создайте новый ID приложения**.
    ![3.jpg]({{site.baseurl}}/attachments/ref_fblogin/3.jpg)
    
3.	В поле **Отображаемое название** укажите название приложения. Его увидят пользователи, поэтому рекомендуется включить в него название магазина. 
	В поле **Эл. адрес для связи** напишите адрес электронной почты, который вы будете использовать для переписки касательно приложения. Нажмите **Создайте ID приложения**.
    
4.  Откроется новое окно **Проверка безопасности**. Введите код с картинки и нажмите **Отправить**. 
    ![4.jpg]({{site.baseurl}}/attachments/ref_fblogin/4.jpg)

5.  Откроется страница выбора нового продукта. Наведите курсор на **Вход через Facebook** и нажмите **Настроить**:
	![5.jpg]({{site.baseurl}}/attachments/ref_fblogin/5.jpg)
    
6.  Выберите платформу:
	![6.jpg]({{site.baseurl}}/attachments/ref_fblogin/6.jpg)
    
    Запускается мастер настройки нового приложения.

7.  На первом шаге настройки укажите веб-адрес сайта, нажмите **Save** и **Продолжить**:
    ![7.jpg]({{site.baseurl}}/attachments/ref_fblogin/7.jpg)
        
8.  Последующие шаги можно пропустить, т.к. они настраиваются модулем **Social Login**.
	![facebook_5.png]({{site.baseurl}}/attachments/ref_vpEKPoyM/facebook_5.png)

9.	На странице **Настройки** заполните поля **URL-адрес политики конфиденциальности** и **URL-адрес Пользовательского соглашения** (это ссылки на соответствующие страницы в магазине), и выберите категорию приложения **Бизнес и Страницы**. Нажмите **Сохранить изменения**:
    ![facebook_dashboard.png]({{site.baseurl}}/attachments/ref_vpEKPoyM/facebook_dashboard.png)
     
10.  Пока приложение находится на стадии разработки, оно не действует на сайте. Перейдите на страницу **Проверка приложения** и сделайте приложение доступным для всех:
    ![development.png]({{site.baseurl}}/attachments/ref_vpEKPoyM/development.png)
    
    Подтвердите действие:
    ![popup.png]({{site.baseurl}}/attachments/ref_vpEKPoyM/popup.png)

    Приложение опубликовано:
    ![public.png]({{site.baseurl}}/attachments/ref_vpEKPoyM/public.png)

    Настройка приложения завершена.

## Настройка модуля Social Login и Facebook

Откройте панель управления X-Cart в новой вкладке или новом окне браузера, чтобы легко переключаться между магазином и Facebook.

1.  На странице **Мои модули** найдите модуль **Social login**:
    ![]({{site.baseurl}}/attachments/7504575/9439791.png)
    
    Откройте настройки модуля:
    ![sociallogin.png]({{site.baseurl}}/attachments/ref_vpEKPoyM/sociallogin.png)
    
2.  Заполните поля **Facebook App ID/API Key** (Идентификатор приложения) и **Facebook App Secret** (Секрет приложения). Для этого скопируйте **Идентификатор приложения** и **Секрет приложения** со страницы **Панель** в Facebook. Для просмотра секрета нажмите **Показать**, введите свой пароль для Facebook и нажмите **Отправить**. 

	Включите или отключите опцию **Request user location**. Для чего она нужна: модуль **Social login** запрашивает информацию о местонахождении пользователя, на получение которой требуется подтверждение от Facebook. Если пользователь указал свое местонахождение в профиле в Facebook и X-Cart получил эту информацию, при авторизации покупателя в магазине его адрес подставляется автоматически.

3.  Когда все данные Facebook внесены, нажмите **Сохранить**.

    Теперь на странице входа в магазин покупатели увидят кнопку **Войти через Facebook**.

_Дополнительная информация:_

*   {% link "Social Login" ref_IapN8lJ8 %}
*   {% link "Setting up Google Login for your store" ref_LMCQeIrv %}