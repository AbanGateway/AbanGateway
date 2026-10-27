<div align="center">

<img src="assets/banner.png" alt="آبان گیت وی: پرداخت کارت به کارت، خودکار تایید میشود" width="100%">

<!-- Latin labels on purpose: shields.io draws badge text without a Persian
     font or bidi, so a Persian label comes out reordered. -->
[![website](https://img.shields.io/badge/website-abangateway.ir-1F6FEB?style=for-the-badge)](https://abangateway.ir)
[![docs](https://img.shields.io/badge/docs-AbanGateway%2Fdocs-27E0FF?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AbanGateway/docs)
[![bot](https://img.shields.io/badge/bot-@Abangw__bot-229ED9?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/Abangw_bot)
[![channel](https://img.shields.io/badge/channel-@abangateway-229ED9?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/abangateway)

</div>

## 👋 آبان گیت وی

درگاه پرداخت کارت به کارت که پرداخت را خودش تایید میکند. خریدار به کارت فروشنده کارت به کارت میکند، بانک به گوشی فروشنده پیامک میزند، و ما همان پیامک را میخوانیم و فاکتور را میبندیم.

پول از اول تا آخر مستقیم به کارت خود فروشنده میرود. نه درگاه بانکی لازم است، نه نماد اعتماد، نه قرارداد.

<div dir="rtl">

| 🧾 فاکتور | 💳 کارت به کارت | ✅ تایید خودکار |
|:---:|:---:|:---:|
| هر سفارش یک مبلغ یکتا میگیرد | خریدار مستقیم به کارت فروشنده میزند | پیامک بانک خوانده میشود و وبهوک میرسد |

</div>

## 🧭 از کجا شروع کنم

<table dir="rtl">
<tr>
<td width="33%" valign="top">

**🛍 سایت ندارم**<br>
[لینک پرداخت](https://github.com/AbanGateway/docs/blob/main/integrations/payment-links.md)، برای فروش در اینستاگرام و تلگرام

</td>
<td width="33%" valign="top">

**🌐 سایت دارم**<br>
[ووکامرس](https://github.com/AbanGateway/docs/blob/main/integrations/woocommerce.md) · [WHMCS](https://github.com/AbanGateway/docs/blob/main/guides/whmcs.md) · [لاراول](https://github.com/AbanGateway/docs/blob/main/integrations/laravel.md)

</td>
<td width="33%" valign="top">

**🤖 ربات تلگرام دارم**<br>
[میرزا](https://github.com/AbanGateway/docs/blob/main/integrations/mirza-pro.md) · [فاکسیما](https://github.com/AbanGateway/docs/blob/main/integrations/faoxima.md) · [DDbot](https://github.com/AbanGateway/docs/blob/main/integrations/ddbot.md) · [ویزویز](https://github.com/AbanGateway/docs/blob/main/integrations/wizwiz.md)

</td>
</tr>
<tr>
<td valign="top">

**👨‍💻 برنامه نویسم**<br>
[مرجع API](https://github.com/AbanGateway/docs/blob/main/api/README.md) · [بسته PHP و لاراول](https://packagist.org/packages/abangateway/abangateway-php-package)

</td>
<td valign="top">

**📱 گوشی فروشنده**<br>
[اپ اندروید](https://github.com/AbanGateway/docs/blob/main/integrations/forwarder-app.md) · [آیفون، با اینترنت یا بدون اینترنت](https://github.com/AbanGateway/docs/blob/main/guides/iphone-shortcut.md)

</td>
<td valign="top">

**🌱 تازه ام**<br>
[از صفر تا اولین پرداخت](https://github.com/AbanGateway/docs/blob/main/guides/start.md)

</td>
</tr>
</table>

## 👨‍💻 برای برنامه نویس ها

یک درخواست فاکتور میسازد و یک لینک پرداخت برمیگرداند. وقتی پول نشست، وبهوک به سایت شما میرسد.

```bash
curl -X POST https://api.abangateway.ir/api/v1/invoices \
  -H "Authorization: Bearer $ABAN_TOKEN" \
  -H "Content-Type: application/json" \
  -d '{"amount_rial": 5990000, "order_id": "ORD-1043",
       "callback_url": "https://shop.example/hook"}'
```

با PHP و لاراول:

```bash
composer require abangateway/abangateway-php-package
```

## 📦 مخزن ها

<div dir="rtl">

| مخزن | چه چیزی |
|---|---|
| [docs](https://github.com/AbanGateway/docs) | مستندات کامل: API، وبهوک، اتصال ها و راهنمای فروشنده |
| [abangateway-php-package](https://github.com/AbanGateway/abangateway-php-package) | بسته رسمی PHP و لاراول، روی Packagist |

</div>

<div align="center">
<sub><a href="https://abangateway.ir">abangateway.ir</a> · ربات <a href="https://t.me/Abangw_bot">@Abangw_bot</a> · کانال <a href="https://t.me/abangateway">@abangateway</a></sub>
</div>
