---
lang: ru
layout: article_with_sidebar
updated_at: '2017-11-14 15:19 +0400'
identifier: ref_BhDJ3y0W
title: 'Импорт CSV: Заказы'
order: 60
published: false
---
{% note info %}
Функциональность импорта заказов является частью функциональности бесплатного модуля [Orders Import](https://market.x-cart.com/addons/orders-import.html). Она не входит в ядро X-Cart.
{% endnote %}

В таблице ниже представлены поля, которые можно импортировать, и их содержание.

<table class="ui celled padded compact small table">
  <thead>
    <tr>
      <th class="confluenceTh">Поле в CSV файле</th>
      <th colspan="1" class="confluenceTh">Что описывает это поле</th>
      <th colspan="1" class="confluenceTh" markdown="1">{% link 'Тип значения' ref_2LwMTTTW %}</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td colspan="3" class="confluenceTd"><em> Поля, поддерживаемые модулем <strong>Orders Import</strong></em>
      </td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>orderNumber*</strong>
      </td>
      <td colspan="1" class="confluenceTd">Номер заказа.Служит идентификатором покупки.</td>
      <td colspan="1" class="confluenceTd">
        <p>Целое число</p>
      </td>
    </tr>
    <tr>
      <td colspan="3" class="confluenceTd">Поля адреса оплаты покупателя. Следующие поля могут быть представлены или не представлены в вашем магазине в зависимости от конфигурации записи адресов.
      </td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerAnonymous</td>
      <td colspan="1" class="confluenceTd">Если значение Yes, покупатель - незарегистрированный (анонимный) пользователь.</td>
      <td colspan="1" class="confluenceTd">Да/Нет</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerAddressSame</td>
      <td colspan="1" class="confluenceTd">Поставьте Yes, если адреса оплаты и доставки покупателя совпадают. Если не совпадают - поставьте No.</td>
      <td colspan="1" class="confluenceTd">Да/Нет</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerFirstnameBillingAddressField</td>
      <td colspan="1" class="confluenceTd">Имя покупателя в адресе оплаты.<br> </td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerLastnameBillingAddressField</td>
      <td colspan="1" class="confluenceTd">Фамилия покупателя в адресе оплаты</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerStreetBillingAddressField</td>
      <td colspan="1" class="confluenceTd">Улица в адресе оплаты</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerCityBillingAddressField</td>
      <td colspan="1" class="confluenceTd">Город в адресе оплаты</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerCountryCodeBillingAddressField</td>
      <td colspan="1" class="confluenceTd">Код страны (в формате ISO 3166-1 alpha-2 (два знака)) в адресе оплаты</td>
      <td colspan="1" class="confluenceTd">Текст,<br>Максимум 2 знака</td>
    </tr>

    <tr>
      <td colspan="1" class="confluenceTd">customerStateIdBillingAddressField</td>
      <td colspan="1" class="confluenceTd">Название области, если в конфигурации магазина указана такая область. Если не указана, заполните поле customerCustomStateBillingAddressField. <br> Пример: Иркутская Область.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerCustomStateBillingAddressField</td>
      <td colspan="1" class="confluenceTd">Название области, если в конфигурации магазина не указана область из адреса покупателя. </td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerZipcodeBillingAddressField</td>
      <td colspan="1" class="confluenceTd">Индекс в адресе оплаты.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerPhoneBillingAddressField</td>
      <td colspan="1" class="confluenceTd">Номер телефона покупателя в адресе оплаты.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerVatNumberBillingAddressField</td>
      <td colspan="1" class="confluenceTd"></td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="3" class="confluenceTd">Поля адрес доставки покупателя.  Следующие поля могут быть представлены или не представлены в вашем магазине в зависимости от конфигурации записи адресов.</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerFirstnameShippingAddressField</td>
      <td colspan="1" class="confluenceTd">Имя покупателя в адресе доставки.<br> </td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerLastnameShippingAddressField</td>
      <td colspan="1" class="confluenceTd">Фамилия покупателя в адресе доставки</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerStreetShippingAddressField</td>
      <td colspan="1" class="confluenceTd">Улица в адресе доставки</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerCityShippingAddressField</td>
      <td colspan="1" class="confluenceTd">Город в адресе доставки</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerCountryCodeShippingAddressField</td>
      <td colspan="1" class="confluenceTd">Код страны (в формате ISO 3166-1 alpha-2 (два знака)) в адресе доставки</td>
      <td colspan="1" class="confluenceTd">Текст,<br>Max. length: 2</td>
    </tr>

    <tr>
      <td colspan="1" class="confluenceTd">customerStateIdShippingAddressField</td>
      <td colspan="1" class="confluenceTd">Название области, если в конфигурации магазина указана такая область. Если не указана, заполните поле customerCustomStateShippingAddressField. <br>Пример: Иркутская Область</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerCustomStateShippingAddressField</td>
      <td colspan="1" class="confluenceTd">Название области, если в конфигурации магазина не указана область из адреса покупателя. </td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerZipcodeShippingAddressField</td>
      <td colspan="1" class="confluenceTd">Индекс в адресе доставки.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerPhoneShippingAddressField</td>
      <td colspan="1" class="confluenceTd">Номер телефона в адресе доставки.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">customerVatNumberShippingAddressField</td>
      <td colspan="1" class="confluenceTd"></td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="3" class="confluenceTd">Поля покупаемых продуктов. Каждое поле содержит несколько рядов, и каждый ряд представляет отдельный продукт.</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>itemName*</strong></td>
      <td colspan="1" class="confluenceTd">Название покупаемого продукта.</td>
      <td colspan="1" class="confluenceTd">Текст,<br>Несколько рядов</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>itemSKU*</strong></td>
      <td colspan="1" class="confluenceTd">Артикул покупаемого продукта.</td>
      <td colspan="1" class="confluenceTd">Текст,<br>Несколько рядов,<br>Максимум 32 знака</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">itemAttributes</td>
      <td colspan="1" class="confluenceTd">Атрибуты покупаемого продукта.</td>
      <td colspan="1" class="confluenceTd">Несколько значений,<br>Несколько рядов</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>itemPrice*</strong></td>
      <td colspan="1" class="confluenceTd">Розничная цена продукта.</td>
      <td colspan="1" class="confluenceTd">Плавающая величина,<br>Несколько рядов</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>itemQuantity*</strong></td>
      <td colspan="1" class="confluenceTd">Количество продукта в заказе.</td>
      <td colspan="1" class="confluenceTd">Целое чсло,<br>Несколько рядов</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>itemSubtotal*</strong></td>
      <td colspan="1" class="confluenceTd">Промежуточная стоимость продукта (без учета наценок).</td>
      <td colspan="1" class="confluenceTd">Плавающая величина,<br>Несколько рядов</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>itemTotal*</strong></td>
      <td colspan="1" class="confluenceTd">Полная стоимость продукта.</td>
      <td colspan="1" class="confluenceTd">Плавающая величина,<br>Несколько рядов</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>subtotal*</strong></td>
      <td colspan="1" class="confluenceTd">Промежуточная сумма заказа (без учета наценок).</td>
      <td colspan="1" class="confluenceTd">Плавающая величина</td>
    </tr>
    <tr>
      <td colspan="3" class="confluenceTd">Наценки на заказы. В каждом поле наценки указан код наценки (большими буквами) и суффикс наценки. Пример наценки на заказ можно увидеть в двух следующих поля. В зависимости от конфигурации вашего магазина, такие же поля могут быть представлены или нет.</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">DISCOUNT (surcharge)</td>
      <td colspan="1" class="confluenceTd">Абсолютная величина скидки на заказ. Пример: -100. Это означает, что на заказ действует скидка RUB100, если валюта заказа - RUB.</td>
      <td colspan="1" class="confluenceTd">Плавающая величина</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">SHIPPING (surcharge)</td>
      <td colspan="1" class="confluenceTd">Наценка на доставку. Пример: 150.</td>
      <td colspan="1" class="confluenceTd">Плавающая величина</td>
    </tr>    
    <tr>
      <td colspan="1" class="confluenceTd"><strong>total*</strong></td>
      <td colspan="1" class="confluenceTd">Полная сумма заказа со всеми доплатами.</td>
      <td colspan="1" class="confluenceTd">Плавающая величина</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>currency*</strong></td>
      <td colspan="1" class="confluenceTd">Код валюты заказа. Пример: RUB.</td>
      <td colspan="1" class="confluenceTd">Текст,<br>Максимум 3 знака</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">shippingMethod</td>
      <td colspan="1" class="confluenceTd">Название способа доставки заказа.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">trackingNumber</td>
      <td colspan="1" class="confluenceTd">Номер отслеживания заказа.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="3" class="confluenceTd">Платежные транзакции по заказу. Следующие поля с префиксом paymentTransaction содержат несколько рядов, и каждый ряд содержит одну транзакцию.</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>paymentTransactionMethod*</strong></td>
      <td colspan="1" class="confluenceTd">Внутреннее название способа оплаты заказа.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>paymentTransactionStatus*</strong></td>
      <td colspan="1" class="confluenceTd">Статус транзакции.<br>
        Возможные значения:
        <ul>
          <li>'I' (Начата оплата)</li>
          <li>'P' (В обработке)</li>
          <li>'S' (Успешная оплата)</li>
          <li>'W' (Незавершённый платеж)</li>
          <li>'F' (Оплата не прошла)</li>
          <li>'C' (Отмена)</li>
          <li>'V' (Аннулирован)</li>
        </ul>
      </td>
      <td colspan="1" class="confluenceTd">Текст,<br>Максимум 1 знак</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>paymentTransactionValue*</strong></td>
      <td colspan="1" class="confluenceTd">Сумма транзакции.</td>
      <td colspan="1" class="confluenceTd">Float</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">paymentTransactionNote</td>
      <td colspan="1" class="confluenceTd">Комментарии платежной системы к транзакции по заказу. Обычно, это сообщения об ошибках при оплате.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>paymentTransactionType*</strong></td>
      <td colspan="1" class="confluenceTd">Тип транзакции.<br>
        Возможные значения:
        <ul>
          <li>'auth' (Только авторизация)</li>
          <li>'sale' (Авторизация и удержание)</li>
          <li>'capture' (Удержание средств)</li>
          <li>'capturePart' (Частичное удержание средств с последующим завершением транзакции)</li>
          <li>'captureMulti' (Частичное удержание средств. Возможно повторение)</li>
          <li>'void' (Платеж аннулирован)</li>
          <li>'voidPart' (Частичная отмена платежа с последующим завершением транзакции)</li>
          <li>'voidMulti' (Частичная отмена платежа. Возможно повторение)</li>
          <li>'refund' (Возврат средств)</li>
          <li>'refundPart' (Частичный возврат средств с последующим завершением транзакции)</li>
          <li>'refundMulti' (Возврат средств. Возможно повторение)</li>
        </ul>
      </td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>paymentTransactionId*</strong></td>
      <td colspan="1" class="confluenceTd">Order payment transaction public id.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>    
    <tr>
      <td colspan="1" class="confluenceTd">paymentTransactionCurrency</td>
      <td colspan="1" class="confluenceTd">Order payment transaction currency. Can be omitted; order currency will be used instead.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>    
    <tr>
      <td colspan="1" class="confluenceTd">date</td>
      <td colspan="1" class="confluenceTd">Order creation date. Example: Tue, 12 Jan 2016 13:18:22 +0000</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>    
    <tr>
      <td colspan="1" class="confluenceTd">recent</td>
      <td colspan="1" class="confluenceTd">Use "Yes" if the order has been processed by the admin, otherwise use "No".</td>
      <td colspan="1" class="confluenceTd">Yes/No</td>
    </tr>    
    <tr>
      <td colspan="1" class="confluenceTd"><strong>paymentStatus*</strong></td>
      <td colspan="1" class="confluenceTd">Order payment status. <br>
        Possible values are:
        <ul>
          <li>'A' (Authorized)</li>
          <li>'P' (Paid)</li>
          <li>'PP' (Partially paid)</li>
          <li>'D' (Declined)</li>
          <li>'C' (Cancelled)</li>
          <li>'Q' (Queued)</li>
          <li>'R' (Refunded)</li>
        </ul>
      </td>
      <td colspan="1" class="confluenceTd">Текст,<br>Max. length: 3</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>shippingStatus*</strong></td>
      <td colspan="1" class="confluenceTd">Order shipping status. <br>
        Possible values are:
        <ul>
          <li>'N' (New order)</li>
          <li>'P' (Processing)</li>
          <li>'S' (Shipped)</li>
          <li>'D' (Delivered)</li>
          <li>'WND' (Will not deliver)</li>
          <li>'WFA' (Waiting for approve)</li>
          <li>'R' (Returned)</li>
        </ul>
      </td>
      <td colspan="1" class="confluenceTd">Текст,<br>Max. length: 3</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">notes</td>
      <td colspan="1" class="confluenceTd">Order customer notes.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">adminNotes</td>
      <td colspan="1" class="confluenceTd">Order administrator notes.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="3" class="confluenceTd">Order history details. The following fields prefixed by 'detail' are Multirow, and each row represents a single history item.
      </td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">detailCode</td>
      <td colspan="1" class="confluenceTd">Order history item code</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">detailLabel</td>
      <td colspan="1" class="confluenceTd">Order history item human-readable label</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">detailValue</td>
      <td colspan="1" class="confluenceTd">Order history item text.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="3" class="confluenceTd"><em> Fields added by the <strong>Multivendor addon</strong></em>
      </td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>vendor*</strong>
      </td>
      <td colspan="1" class="confluenceTd">Order vendor email.</td>
      <td colspan="1" class="confluenceTd">Текст</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>parent*</strong>
      </td>
      <td colspan="1" class="confluenceTd">Parent order ID.</td>
      <td colspan="1" class="confluenceTd">Integer</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd"><strong>children*</strong>
      </td>
      <td colspan="1" class="confluenceTd">Child order numbers. Can be multiple.</td>
      <td colspan="1" class="confluenceTd">Integer,<br>Multiple</td>
    </tr>
    <tr>
      <td colspan="3" class="confluenceTd"><em> Fields added by the <strong>Custom Order Statuses addon</strong></em>
      </td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">paymentStatusLabel</td>
      <td colspan="1" class="confluenceTd">Human-readable translation of the payment status</td>
      <td colspan="1" class="confluenceTd">Текст,<br>Multilingual</td>
    </tr>
    <tr>
      <td colspan="1" class="confluenceTd">shippingStatusLabel</td>
      <td colspan="1" class="confluenceTd">Human-readable translation of the shipping status</td>
      <td colspan="1" class="confluenceTd">Текст,<br>Multilingual</td>
    </tr>
  </tbody>
</table>

<sub>* Required field.</sub>

<sub markdown="1">** See CSV field attributes for more info.</sub>

**Tips**:

*   If you are going to import data into X-Cart and do not wish to update certain X-Cart fields during the import process, you should not include these fields into your CSV file for import. Simply remove the respective column(s) from the file.
