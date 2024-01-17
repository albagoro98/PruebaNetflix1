Delivered-To: albagoro98@gmail.com
Received: by 2002:a05:7208:809c:b0:7c:38e7:6d02 with SMTP id k28csp798909rbd;
        Wed, 10 Jan 2024 08:59:45 -0800 (PST)
X-Google-Smtp-Source: AGHT+IELlh/djXodOOgedClvCQ/goS+qY1ZkHW5xOp4s0zaxhajIIwufbh+GtfdOt8K2Ws1pdPck
X-Received: by 2002:a67:f5ca:0:b0:467:c9d4:d935 with SMTP id t10-20020a67f5ca000000b00467c9d4d935mr2092705vso.1.1704905985264;
        Wed, 10 Jan 2024 08:59:45 -0800 (PST)
ARC-Seal: i=1; a=rsa-sha256; t=1704905985; cv=none;
        d=google.com; s=arc-20160816;
        b=mrVs5+x1NEZaeOjp6W0kNnQ6IPQQopW120xhsS922PjyXZRt/ho5cfCqgu/3HAJg5q
         4/VlOvRrCST21TnXCoUzv4TeEq4p+pDD2E93leL+FX/NdYWpp4+zAvZ7S0dfxWSBTWJ8
         aD2D+UUVKqUnH8OXYOsIpzOAdBlThBc5HT6dRYoW6qu6omkz41xroBoZY7UIdHiWEYoX
         bRQpRhPIkEq0tyEeyrz3PN1yo6J0YmVilKjjRgkFgLOe18+Ed1rZLIDKzr4DOhQzcFkb
         KU4ccsf3BdUdLN/xwHTnRkBRXl397nSEAk4Ysg3sFW+xmmIfsy6Oiaqn+/3nzH44DhxB
         sT3Q==
ARC-Message-Signature: i=1; a=rsa-sha256; c=relaxed/relaxed; d=google.com; s=arc-20160816;
        h=feedback-id:list-unsubscribe:mime-version:subject:message-id:to
         :from:date:dkim-signature:dkim-signature;
        bh=NBRywwEwPseYzmRwXli0SBqMlDBUaasRHaYRIThwxVQ=;
        fh=GLPZ/FTgbNbftLDKuTB66Il4/4FjoCjlxKs/lm+q2+A=;
        b=tuqEoBeky9vCFiCnH1HjCrR9XlfjbbxDA4kmOUJhZPANGVi4+vko8EVI0/A0WqYr35
         8pxUtv83KT56lQhZXZZxKYguOVPaomob45C5v0fUYDBiSFjwqrzT77ul+L41Mjv8dcBC
         tMxAkaBSRfgrrRCw01QSd7IHSOMrsIN6xXZ08PyrEy/im7yWgfM7LX9FaLI6jmjgVErC
         RPLegKY+PI3H0BpjTihVB29Ya1DJphMRLMRiVHNnz819lebB7r7sFPwb8cFfYkV3oCBq
         naR9Ka3P/B85N8yTSZ3zHw8HfKxYlXTpRjeGzLTVS1oC9oF64tGKeG7UPD0yGg1bW3Uq
         Un2A==
ARC-Authentication-Results: i=1; mx.google.com;
       dkim=pass header.i=@account.netflix.com header.s=uwy7ntyrpcutc5u6vby7zselewc4ildi header.b=4xzHDXzP;
       dkim=pass header.i=@amazonses.com header.s=224i4yxa5dv7c2xz3womw6peuasteono header.b=Z0fftk2L;
       spf=pass (google.com: domain of 0100018cf450cae5-228c0b4f-d408-4013-b275-5f4d775559cb-000000@mailer.account.netflix.com designates 54.240.77.120 as permitted sender) smtp.mailfrom=0100018cf450cae5-228c0b4f-d408-4013-b275-5f4d775559cb-000000@mailer.account.netflix.com;
       dmarc=pass (p=REJECT sp=REJECT dis=NONE) header.from=netflix.com
Return-Path: <0100018cf450cae5-228c0b4f-d408-4013-b275-5f4d775559cb-000000@mailer.account.netflix.com>
Received: from a77-120.smtp-out.amazonses.com (a77-120.smtp-out.amazonses.com. [54.240.77.120])
        by mx.google.com with ESMTPS id bx11-20020a05622a090b00b004299991042bsi4519054qtb.644.2024.01.10.08.59.45
        for <albagoro98@gmail.com>
        (version=TLS1_2 cipher=ECDHE-ECDSA-AES128-GCM-SHA256 bits=128/128);
        Wed, 10 Jan 2024 08:59:45 -0800 (PST)
Received-SPF: pass (google.com: domain of 0100018cf450cae5-228c0b4f-d408-4013-b275-5f4d775559cb-000000@mailer.account.netflix.com designates 54.240.77.120 as permitted sender) client-ip=54.240.77.120;
Authentication-Results: mx.google.com;
       dkim=pass header.i=@account.netflix.com header.s=uwy7ntyrpcutc5u6vby7zselewc4ildi header.b=4xzHDXzP;
       dkim=pass header.i=@amazonses.com header.s=224i4yxa5dv7c2xz3womw6peuasteono header.b=Z0fftk2L;
       spf=pass (google.com: domain of 0100018cf450cae5-228c0b4f-d408-4013-b275-5f4d775559cb-000000@mailer.account.netflix.com designates 54.240.77.120 as permitted sender) smtp.mailfrom=0100018cf450cae5-228c0b4f-d408-4013-b275-5f4d775559cb-000000@mailer.account.netflix.com;
       dmarc=pass (p=REJECT sp=REJECT dis=NONE) header.from=netflix.com
DKIM-Signature: v=1; a=rsa-sha256; q=dns/txt; c=relaxed/simple; s=uwy7ntyrpcutc5u6vby7zselewc4ildi; d=account.netflix.com; t=1704905984; h=Date:From:To:Message-ID:Subject:MIME-Version:Content-Type:List-Unsubscribe; bh=57vfHOvvVz/BIzDLn5YIZtXbV1Y3PWf4kTKOm08/pm0=; b=4xzHDXzPvp9lK62Aw6Ed9YxTdKe1VW6CE2fpzl0dQoNZB+gPqLUETvo9MLxEVKEx TZhJe0YRQHXEFleg7OSwBmRW4XP3by6wllcfDLojn5w/tsZFfBCgDNUXiMXpuX4vzSU 8q5A2UgEh9Opcc4lkLF1P3B8b7Yj6CPu9yW5MEcg=
DKIM-Signature: v=1; a=rsa-sha256; q=dns/txt; c=relaxed/simple; s=224i4yxa5dv7c2xz3womw6peuasteono; d=amazonses.com; t=1704905984; h=Date:From:To:Message-ID:Subject:MIME-Version:Content-Type:List-Unsubscribe:Feedback-ID; bh=57vfHOvvVz/BIzDLn5YIZtXbV1Y3PWf4kTKOm08/pm0=; b=Z0fftk2LdxsYw9lliGqduXB4LRqF/95r+Q1qYlozEakJZ9PVEkF3ipuQc4mfoPqY ZZv+jOT09OlxgR0mcbx7jQb1Sz+QRBcHU76ke+f+UZ5IaAr14QmBhh3dD3Cm4Lmch46 i3U0h24i8yXoeA7ecrvyDHxEZEDOlUlLoWdJZFkg=
Date: Wed, 10 Jan 2024 16:59:44 +0000
From: Netflix <info@account.netflix.com>
To: albagoro98@gmail.com
Message-ID: <0100018cf450cae5-228c0b4f-d408-4013-b275-5f4d775559cb-000000@email.amazonses.com>
Subject: Completar tu solicitud de cambio de contraseña
MIME-Version: 1.0
Content-Type: multipart/alternative; boundary="----=_Part_118186_1531067444.1704905984720"
X-TrackingUuid: adcac973-9bc0-4ca8-860e-af0c1eef9137
X-AppInfo: easel::us-east-1::1::easel-i-06c65c925bf6008c3::prod
X-WorkflowId: 61B78492
X-MessageGuid: c2dd2aad-7647-480a-b786-7810c37e1534
List-Unsubscribe: <mailto:TlVYM1ZUM0xXVkRMVkJTU0hWN0lBM0JQWk0zNDc0@unsubscribe.netflix.com>, <https://www.netflix.com/notificationsettings/email?id=BQE0AAEBECOicK1LEvsmMBlrZpPOoMSAkL7Ae2xDr5SvB8xuS5GNANognyHYUQiMaNTA4tLYyi3iTvHuvlAk%2BgA7H%2BihDgfLs44dW3S4mcKaFaO0eyW%2Fjr10pukTHT57gJA5joYgQqbDElCz%2FhAS6wf5ZYgF8XTXhNTQYy6Sbrr8DkKgC0P6V5tO4n73%2BJO%2Ff2CDdYbpFC1oI4fH9zUrwS%2B2a5pnslc7XA%3D%3D&lnktrk=EVO&g=c2dd2aad-7647-480a-b786-7810c37e1534&lkid=unsubscribe_link>
X-localeCountry: es-ES::ES
X-To: albagoro98@gmail.com
X-SourceAppName: dynecom
X-TaskUuid: 0d612c61-6751-483d-b3d0-190c2c887238
X-EventGuid: adcac973-9bc0-4ca8-860e-af0c1eef9137
X-ProcEnc: BQAtAAEBEKDQAbNs6G4Y0YA0CjfXsQQg53GSuFpUiIrNoerhpM/jSrcBamfADVlU5cZtG1UyLXs=
Feedback-ID: 1.us-east-1.cH2tGwpBLIxia3teqeNiC4px/mCp35LHVs2n0ZR/rKI=:AmazonSES
X-SES-Outgoing: 2024.01.10-54.240.77.120

------=_Part_118186_1531067444.1704905984720
Content-Type: text/plain; charset=UTF-8
Content-Transfer-Encoding: quoted-printable

Cambia tu contrase=C3=B1a

Cambia tu contrase=C3=B1a

Hola, Alba:

Cambia tu contrase=C3=B1a para que puedas volver a ver contenidos
en Netflix.

Restablecer contrase=C3=B1a
[https://www.netflix.com/password?g=3Dc2dd2aad-7647-480a-b786-7810c37e1534&=
lkid=3DURL_CTA&lnktrk=3DEVO&nftoken=3DBQAbAAEBEE3gzcF2xRaFaWzzbjaIFD6AoCP9u=
3eUEN%2F5yolxsJrvPO4grPry22UJoV8SSvUtqUNQmFBDBn6UMMtHgJit9X%2FenA0JtsUYz8wb=
iFYSb4qdekudZXprxJJmW8rbFuflsEOlYmqbcDQWfdh9FoeSuqkpi4UzO%2FOJ2QrnKwljRwNm4=
9gGJlgcySExB%2FemMPOas3NOPXAQD55Py8bHkZsIWy%2BqD0RsmarxKhIC86uwBt4oFrY%3D]

Si no has solicitado que cambiemos tu contrase=C3=B1a, te
recomendamos que revises los accesos recientes a tu cuenta
[https://www.netflix.com/accountaccess?g=3Dc2dd2aad-7647-480a-b786-7810c37e=
1534&lkid=3DURL_ACCOUNT_ACCESS&lnktrk=3DEVO]
para detectar cualquier actividad extra=C3=B1a.

Estamos aqu=C3=AD para ayudarte cuando lo necesites. Visita el
Centro de ayuda
[https://help.netflix.com/support/365?g=3Dc2dd2aad-7647-480a-b786-7810c37e1=
534&lkid=3DURL_HELP&lnktrk=3DEVO]
si quieres m=C3=A1s informaci=C3=B3n o ponte en contacto con nosotros
[https://help.netflix.com/contactus?g=3Dc2dd2aad-7647-480a-b786-7810c37e153=
4&lkid=3DURL_CONTACT&lnktrk=3DEVO].

El equipo de Netflix

=C2=A0
=C2=A0

   =C2=BFPreguntas? Llama al 900-759-106
  =20
   Netflix Servicios de Transmisi=C3=B3n Espa=C3=B1a, S.L.
   [https://help.netflix.com/legal/corpinfo?g=3Dc2dd2aad-7647-480a-b786-781=
0c37e1534&lkid=3DURL_CORP_INFO&lnktrk=3DEVO]
  =20
   Configuraci=C3=B3n de comunicaci=C3=B3n
   [https://www.netflix.com/ManageSubscriptions?g=3Dc2dd2aad-7647-480a-b786=
-7810c37e1534&lkid=3DURL_COMM_SETTINGS&lnktrk=3DEVO&id=3DBQE0AAEBECOicK1LEv=
smMBlrZpPOoMSAkL7Ae2xDr5SvB8xuS5GNANognyHYUQiMaNTA4tLYyi3iTvHuvlAk%2BgA7H%2=
BihDgfLs44dW3S4mcKaFaO0eyW%2Fjr10pukTHT57gJA5joYgQqbDElCz%2FhAS6wf5ZYgF8XTX=
hNTQYy6Sbrr8DkKgC0P6V5tO4n73%2BJO%2Ff2CDdYbpFC1oI4fH9zUrwS%2B2a5pnslc7XA%3D=
%3D&mid=3Dnone]
   T=C3=A9rminos de uso
   [https://www.netflix.com/TermsOfUse?g=3Dc2dd2aad-7647-480a-b786-7810c37e=
1534&lkid=3DURL_TERMS&lnktrk=3DEVO]
   Privacidad
   [https://www.netflix.com/PrivacyPolicy?g=3Dc2dd2aad-7647-480a-b786-7810c=
37e1534&lkid=3DURL_PRIVACY&lnktrk=3DEVO]
   Centro de ayuda
   [https://help.netflix.com/help?g=3Dc2dd2aad-7647-480a-b786-7810c37e1534&=
lkid=3DURL_HELP&lnktrk=3DEVO]
  =20
   Netflix ha enviado este correo a [albagoro98@gmail.com]
   [https://www.netflix.com/browse?g=3Dc2dd2aad-7647-480a-b786-7810c37e1534=
&lkid=3DURL_EMAIL&lnktrk=3DEVO]
   como parte de tu suscripci=C3=B3n a Netflix.=C2=A0
   SRC:
   61B78492_c2dd2aad-7647-480a-b786-7810c37e1534_es-ES_ES_EVO
   [https://www.netflix.com/browse?g=3Dc2dd2aad-7647-480a-b786-7810c37e1534=
&lkid=3DURL_SRC&lnktrk=3DEVO]
------=_Part_118186_1531067444.1704905984720
Content-Type: text/html; charset=UTF-8
Content-Transfer-Encoding: quoted-printable


    <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional //EN" "http:/=
/www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
    <html xmlns=3D"http://www.w3.org/1999/xhtml" xmlns:o=3D"urn:schemas-mic=
rosoft-com:office:office" style=3D"background-color: #eaeaea; margin-top: 0=
; padding: 0; margin: 0;">
    <head>
      <meta http-equiv=3D"Content-Type" content=3D"text/html charset=3DUTF-=
8">
      <meta name=3D"viewport" content=3D"width=3Ddevice-width, initial-scal=
e=3D1">
      <meta http-equiv=3D"X-UA-Compatible" content=3D"IE=3Dedge">
      <meta name=3D"format-detection" content=3D"telephone=3Dno">
      <style type=3D"text/css">
@media (max-width: 499px) {
  u + .body .inbox-fix,
u + .body .content-shell-table,
u + .body .footer-shell-table,
u + .body .footer {
    min-width: calc(100vw - 8.5vw) !important;
  }

  .mobile-hide,
.ios-hide {
    display: none !important;
  }

  .desktop-hide,
.desktop-hide img {
    display: initial !important;
  }

  table.desktop-hide {
    display: table !important;
  }

  .mobile-100w {
    width: 100% !important;
  }

  .mobile-block {
    display: block !important;
  }

  .mobile-center {
    margin: 0 auto;
    text-align: center !important;
  }

  .inner-padding {
    padding-left: 6% !important;
    padding-right: 6% !important;
  }

  .outside-padding {
    padding-left: 12% !important;
    padding-right: 12% !important;
  }

  .content-padding {
    padding-left: 6% !important;
    padding-right: 6% !important;
  }

  .desktop-hide-max,
.desktop-hide-max img {
    display: initial !important;
  }
}
@media screen and (-webkit-min-device-pixel-ratio: 0) and (max-width: 499px=
) {
  .container.main-border {
    padding: 0 !important;
  }

  .content-shell {
    border: none !important;
  }
}
@media yahoo {
  table {
    border-collapse: collapse;
    table-layout: fixed;
  }

  table table {
    table-layout: auto;
  }
}
.hide-link a,
.iosnonlink a,
.hide-link {
  text-decoration: none !important;
  cursor: text;
}
@media screen {
  @font-face {
    font-family: NetflixSans-Light;
    src: url("https://assets.nflxext.com/us/email/fonts/NetflixSans-Light-O=
pt.woff2");
    font-weight: 300;
  }

  @font-face {
    font-family: NetflixSans-Regular;
    src: url("https://assets.nflxext.com/us/email/fonts/NetflixSans-Regular=
-Opt.woff2");
    font-weight: 400;
  }

  @font-face {
    font-family: NetflixSans-Medium;
    src: url("https://assets.nflxext.com/us/email/fonts/NetflixSans-Medium-=
Opt.woff2");
    font-weight: 700;
  }

  @font-face {
    font-family: NetflixSans-Bold;
    src: url("https://assets.nflxext.com/us/email/fonts/NetflixSans-Bold-Op=
t.woff2");
    font-weight: 700;
  }
}
@media (max-width: 500px) {
  .button-copy a {
    padding: 13px 0px !important;
    width: 100% !important;
  }
}
@media (min-width: 501px) {
  .button-copy a {
    padding: 13px 40px;
  }
}
@media (max-width: 499px) {
  .image .default-image-width img {
    width: 100%;
  }

  .artwork img {
    width: 100% !important;
  }

  .number img {
    width: 100% !important;
  }
}
@media (max-width: 499px) {
  .episode-content-cell {
    width: 40% !important;
  }

  .episode-content-cell-image {
    width: 100% !important;
    height: auto !important;
  }

  .episode-content-cell-progress-bar {
    width: 100% !important;
    height: auto !important;
  }
}
@media (max-width: 499px) {
  .exp-img-1 img {
    width: 70% !important;
  }

  .exp-img-2 {
    padding-left: 20px !important;
  }

  .exp-img-2 img {
    width: 85% !important;
  }

  .exp-img-3 img {
    width: 85% !important;
  }

  .exp-img-4 img {
    width: 85% !important;
  }

  .calendar img {
    width: 85% !important;
    height: auto !important;
  }
}
@media (max-width: 499px) {
  .logo-with-horizontal-date-logo-image-cell {
    width: 60% !important;
  }
}
@media (max-width: 499px) {
  .thumbs-button-image-width {
    width: 80% !important;
  }

  .thumbs-button-cell-spacer {
    width: 6% !important;
  }
}
@media only screen and (max-width: 500px) {
  .module-kar-hero-inner-body-cell {
    width: 88% !important;
  }
}
@media only screen and (max-width: 500px) {
  .module-kar-hero-inner-body-cell {
    width: 88% !important;
  }
}
@media only screen and (max-width: 500px) {
  .module-kar-themed-category-spacer-td {
    height: 12px !important;
  }
}
@media only screen and (max-width: 500px) {
  .right-pencil-image img {
    width: 75% !important;
    height: auto !important;
  }

  .left-pencil-image img {
    width: 85% !important;
    height: auto !important;
  }

  .left-pencil-cell {
    width: 30% !important;
  }

  .right-pencil-cell {
    width: 30% !important;
  }

  .color-page-cell {
    width: 40% !important;
  }

  .printable-logo-image img {
    width: 40% !important;
    height: auto !important;
  }
}
@media only screen and (max-width: 500px) {
  .module-kar-theme-bars-images img {
    width: 100% !important;
    height: auto !important;
  }
}
@media (max-width: 500px) {
  .mosaic-module .middle {
    width: 46% !important;
    padding-right: 4% !important;
    padding-left: 4% !important;
  }

  .mosaic-module .left,
.mosaic-module .right {
    width: 24.8% !important;
  }

  .mosaic-module .component-image.cell,
.mosaic-module .single-button .content-padding {
    padding-top: 15px !important;
  }
}
@media only screen and (max-width: 500px) {
  .main-header-icon-cell {
    width: 12% !important;
  }

  .header-copy-cell {
    width: 85% !important;
  }

  .header-copy-cell-with-profile-icon {
    width: 78% !important;
  }

  .netflix-logo-cell {
    width: 10% !important;
  }
}
@media (max-width: 499px) {
  .evidence-cards-component-image-cell {
    width: 12% !important;
  }
}
@media (max-width: 499px) {
  .evidence-images img {
    width: 100% !important;
    height: auto !important;
  }
}
@media (max-width: 499px) {
  .marker {
    padding: 5px 7px 5px 7px !important;
  }
}
@media (max-width: 499px) {
  .evidence-trailer-component-image-cell {
    width: 12% !important;
  }
}
@media (max-width: 499px) {
  u + .body .gmail-screen {
    background: #000;
    mix-blend-mode: screen;
  }

  u + .body .gmail-difference {
    background: #000;
    mix-blend-mode: difference;
  }
}
@media (max-width: 499px) {
  .mobile-hide-max,
.ios-hide-max {
    display: none !important;
  }

  .inbox-fix {
    display: none;
  }

  .desktop-hide-max,
.desktop-hide-max img {
    display: initial !important;
  }

  table.content-shell-table,
table.footer-shell-table,
.footer {
    width: 100% !important;
  }

  .content {
    width: 100% !important;
  }
}
.footer-shell .footer-link {
  line-height: 20px;
}
@media (max-width: 499px) {
  .color-wrapper {
    width: 100% !important;
  }
}
@media (max-width: 499px) {
  .bullet .indent.true {
    width: 8% !important;
  }

  .bullet .indent.true {
    padding-left: 3% !important;
  }

  .envelope.rtl .bullet .indent.true {
    padding-right: 3% !important;
  }
}
@media (max-width: 499px) {
  .bullet-point {
    line-height: 22px !important;
  }
}
@media (max-width: 768px) {
  .icon {
    padding-top: 4px !important;
  }
}
@media (max-width: 499px) {
  .image .default-image-width img {
    width: 100%;
  }
}
</style>
    </head>
    <body class=3D"body" style=3D"background-color: #eaeaea; margin-top: 0;=
 padding: 0; margin: 0;">
      <div class=3D"hide" style=3D"display: none; width: 0; height: 0; max-=
height: 0; line-height: 0; mso-hide: all; overflow: hidden; visibility: hid=
den;">Cambia tu contrase=C3=B1a<br><div class=3D"hide disabled-plaintext" s=
tyle=3D"display: none; width: 0; height: 0; max-height: 0; line-height: 0; =
mso-hide: all; overflow: hidden; visibility: hidden;">&#8199;&#847; &#8199;=
&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847=
; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8=
199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&=
#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847;=
 &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#81=
99;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#=
847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; =
&#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#819=
9;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#8=
47; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &=
#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199=
;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#84=
7; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#=
8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;=
&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847=
; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8=
199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&=
#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847;=
 &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#81=
99;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#=
847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; =
&#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#819=
9;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#8=
47; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &=
#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199=
;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#84=
7; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#=
8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;=
&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847=
; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8=
199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&=
#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847;=
 &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#81=
99;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#=
847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &#8199;&#847; &shy; &shy; &s=
hy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy;=
 &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &s=
hy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy;=
 &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &s=
hy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy;=
 &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &s=
hy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy;=
 &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &s=
hy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy;=
 &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &s=
hy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy;=
 &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &s=
hy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy;=
 &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &s=
hy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &shy; &nbsp;</div=
></div><table width=3D"100%" border=3D"0" class=3D"envelope default " cellp=
adding=3D"0" cellspacing=3D"0" style=3D"background-color: #eaeaea;" bgcolor=
=3D"#eaeaea"><tbody><tr><td align=3D"center" class=3D"container" style=3D"b=
ackground-color: #eaeaea; margin-top: 0;" bgcolor=3D"#eaeaea"><table align=
=3D"center" border=3D"0" class=3D"content" cellpadding=3D"0" cellspacing=3D=
"0" style=3D"background-color: #ffffff; width: 500px;" width=3D"500" bgcolo=
r=3D"#ffffff"><tbody><tr><td><table class=3D"tracking-pixel disabled-plaint=
ext image" width=3D"100%" data-testid=3D"image" cellpadding=3D"0" cellspaci=
ng=3D"0"><tbody><tr><td class=3D"cell tracking-pixel disabled-plaintext con=
tent-padding" align=3D"center" style=3D"padding-left: 40px; padding-right: =
40px; padding-top: 0;"><img src=3D"https://beaconimages.netflix.net/img/BAQ=
gBEAEawAJ2THSsgosiINnMMOKPnivWcYZ0JApGjqXUT6_njB_nv93SgfLfWpfkxPOUZMiP91vH0=
2b6k63ud1I5YQ4uu42m3MNFqLjq3z05FO48SpTOQjvcWRtQhxJN-kGsC7yY5OquwehaCzb2X_ns=
GrETy6QmnwCp1ek9gVJbqAdjdypRvZwnoMpNq2nCGHnjI50J49ptW0S-d9Whn_VTOL4BiX8UE6A=
TYRs5VHgx0vN9gk-C1lH4urQBkIn5ejkd3rKcMBdL7w1JSphQ7Ar7aI0UYgs0ktaOY--3I4RfOM=
X2iPUBCjsPdDqMLp5J0VTPRqo0jthTMJqRwXwkCe9AVINGyggFwErfLa2H8gVjSDbuJZutmRxKx=
bN4pWUvJvbJx5dIt4cBwwxB-RPVPzP9b15u1HiOM6CHWSYDbCel4drRRFySqw.." alt width=
=3D"0" border=3D"0" class=3D"undefined " style=3D"-ms-interpolation-mode: b=
icubic; border: none; outline: none; border-collapse: collapse; display: bl=
ock;"></td></tr></tbody></table></td></tr><tr><td align=3D"center" class=3D=
"shell"><a href=3D"https://www.netflix.com/browse?g=3Dc2dd2aad-7647-480a-b7=
86-7810c37e1534&amp;lkid=3DURL_LOGO&amp;lnktrk=3DEVO" class=3D"disabled-pla=
intext" data-testid=3D"logo" style=3D"color: inherit;"><table class=3D"logo=
 image" width=3D"100%" data-testid=3D"image" cellpadding=3D"0" cellspacing=
=3D"0"><tbody><tr><td class=3D"cell logo content-padding" align=3D"left" st=
yle=3D"padding-left: 40px; padding-right: 40px; padding-top: 20px;"><img sr=
c=3D"https://assets.nflxext.com/us/email/gem/nflx.png" alt=3D"Netflix" widt=
h=3D"24" border=3D"0" class=3D"undefined " style=3D"-ms-interpolation-mode:=
 bicubic; border: none; outline: none; border-collapse: collapse; display: =
block; border-style: none;"></td></tr></tbody></table></a><table align=3D"l=
eft" width=3D"100%" class=3D"copy-table " data-testid=3D"copy" cellpadding=
=3D"0" cellspacing=3D"0"><tbody><tr><td align=3D"left" class=3D"copy h1 con=
tent-padding" style=3D"padding-left: 40px; padding-right: 40px; font-family=
: NetflixSans-Bold, Helvetica, Roboto, Segoe UI, sans-serif; font-weight: 7=
00; font-size: 36px; line-height: 43px; letter-spacing: -1px; padding-top: =
20px; color: #221f1f;">Cambia tu contrase=C3=B1a</td></tr></tbody></table><=
table align=3D"left" width=3D"100%" class=3D"copy-table " data-testid=3D"co=
py" cellpadding=3D"0" cellspacing=3D"0"><tbody><tr><td align=3D"left" class=
=3D"copy p content-padding" style=3D"padding-left: 40px; padding-right: 40p=
x; font-family: NetflixSans-Regular, Helvetica, Roboto, Segoe UI, sans-seri=
f; font-weight: 400; font-size: 16px; line-height: 21px; padding-top: 20px;=
 color: #221f1f;">Hola, <span class=3D"break-word" style=3D"word-break: bre=
ak-all;">Alba</span>:</td></tr></tbody></table><table align=3D"left" width=
=3D"100%" class=3D"copy-table " data-testid=3D"copy" cellpadding=3D"0" cell=
spacing=3D"0"><tbody><tr><td align=3D"left" class=3D"copy p content-padding=
" style=3D"padding-left: 40px; padding-right: 40px; font-family: NetflixSan=
s-Regular, Helvetica, Roboto, Segoe UI, sans-serif; font-weight: 400; font-=
size: 16px; line-height: 21px; padding-top: 20px; color: #221f1f;">Cambia t=
u contrase=C3=B1a para que puedas volver a ver contenidos en Netflix.</td><=
/tr></tbody></table><table class=3D"single-button mobile-100w " align=3D"ce=
nter" width=3D"100%" data-testid=3D"single-button" cellpadding=3D"0" cellsp=
acing=3D"0"><tbody><tr><td class=3D"content-padding" align=3D"center" style=
=3D"padding-left: 40px; padding-right: 40px; padding-top: 20px;"><table cla=
ss=3D"inner-button border-false" style=3D"background-color: #e50914; border=
-radius: 4px; width: 100%;" cellpadding=3D"0" cellspacing=3D"0" width=3D"10=
0%" bgcolor=3D"#e50914"><tbody><tr><td class=3D"h5 button-td" align=3D"cent=
er" style=3D"font-family: NetflixSans-Bold, Helvetica, Roboto, Segoe UI, sa=
ns-serif; font-weight: 700; font-size: 14px; line-height: 17px; letter-spac=
ing: -0.2px; padding-top: 20px; padding: 14px 40px; color: #ffffff;"><a cla=
ss=3D"h5" href=3D"https://www.netflix.com/password?g=3Dc2dd2aad-7647-480a-b=
786-7810c37e1534&amp;lkid=3DURL_CTA&amp;lnktrk=3DEVO&amp;nftoken=3DBQAbAAEB=
EE3gzcF2xRaFaWzzbjaIFD6AoCP9u3eUEN%2F5yolxsJrvPO4grPry22UJoV8SSvUtqUNQmFBDB=
n6UMMtHgJit9X%2FenA0JtsUYz8wbiFYSb4qdekudZXprxJJmW8rbFuflsEOlYmqbcDQWfdh9Fo=
eSuqkpi4UzO%2FOJ2QrnKwljRwNm49gGJlgcySExB%2FemMPOas3NOPXAQD55Py8bHkZsIWy%2B=
qD0RsmarxKhIC86uwBt4oFrY%3D" style=3D"font-family: NetflixSans-Bold, Helvet=
ica, Roboto, Segoe UI, sans-serif; font-weight: 700; font-size: 14px; line-=
height: 17px; letter-spacing: -0.2px; text-align: center; text-decoration: =
none; display: block; color: #ffffff;">Restablecer contrase=C3=B1a</a></td>=
</tr></tbody></table></td></tr></tbody></table><table align=3D"left" width=
=3D"100%" class=3D"copy-table " data-testid=3D"copy" cellpadding=3D"0" cell=
spacing=3D"0"><tbody><tr><td align=3D"left" class=3D"copy p content-padding=
" style=3D"padding-left: 40px; padding-right: 40px; font-family: NetflixSan=
s-Regular, Helvetica, Roboto, Segoe UI, sans-serif; font-weight: 400; font-=
size: 16px; line-height: 21px; padding-top: 20px; color: #221f1f;">Si no ha=
s solicitado que cambiemos tu contrase=C3=B1a, te recomendamos que revises =
los <a href=3D"https://www.netflix.com/accountaccess?g=3Dc2dd2aad-7647-480a=
-b786-7810c37e1534&amp;lkid=3DURL_ACCOUNT_ACCESS&amp;lnktrk=3DEVO" style=3D=
"color: inherit; text-decoration: underline;">accesos recientes a tu cuenta=
</a> para detectar cualquier actividad extra=C3=B1a.</td></tr></tbody></tab=
le><table align=3D"left" width=3D"100%" class=3D"copy-table " data-testid=
=3D"copy" cellpadding=3D"0" cellspacing=3D"0"><tbody><tr><td align=3D"left"=
 class=3D"copy p content-padding" style=3D"padding-left: 40px; padding-righ=
t: 40px; font-family: NetflixSans-Regular, Helvetica, Roboto, Segoe UI, san=
s-serif; font-weight: 400; font-size: 16px; line-height: 21px; padding-top:=
 20px; color: #221f1f;">Estamos aqu=C3=AD para ayudarte cuando lo necesites=
. Visita el <a href=3D"https://help.netflix.com/support/365?g=3Dc2dd2aad-76=
47-480a-b786-7810c37e1534&amp;lkid=3DURL_HELP&amp;lnktrk=3DEVO" style=3D"co=
lor: inherit; text-decoration: underline;">Centro de ayuda</a> si quieres m=
=C3=A1s informaci=C3=B3n o <a href=3D"https://help.netflix.com/contactus?g=
=3Dc2dd2aad-7647-480a-b786-7810c37e1534&amp;lkid=3DURL_CONTACT&amp;lnktrk=
=3DEVO" style=3D"color: inherit; text-decoration: underline;">ponte en cont=
acto con nosotros</a>.</td></tr></tbody></table><table align=3D"left" width=
=3D"100%" class=3D"copy-table " data-testid=3D"copy" cellpadding=3D"0" cell=
spacing=3D"0"><tbody><tr><td align=3D"left" class=3D"copy h5 medium content=
-padding" style=3D"padding-left: 40px; padding-right: 40px; font-size: 14px=
; line-height: 17px; letter-spacing: -0.2px; font-family: NetflixSans-Mediu=
m, Helvetica, Roboto, Segoe UI, sans-serif; font-weight: 700; padding-top: =
20px; color: #221f1f;">El equipo de Netflix</td></tr></tbody></table><table=
 width=3D"100%" data-testid=3D"divider" cellpadding=3D"0" cellspacing=3D"0"=
><tbody><tr><td class=3D"divider content-padding" style=3D"padding-left: 40=
px; padding-right: 40px; padding-top: 30px;"><table align=3D"center" width=
=3D"100%" cellpadding=3D"0" cellspacing=3D"0"><tbody><tr><td class=3D"empty=
 divider-border" style=3D"font-size: 0; line-height: 0; border-style: solid=
; border-bottom-width: 0; border-color: #221F1F; border-top-width: 2px;">=
=C2=A0</td></tr></tbody></table></td></tr></tbody></table></td></tr><tr><td=
 align=3D"center" class=3D"footer-shell" style=3D"background-color: #ffffff=
;" bgcolor=3D"#ffffff"><table class=3D"footer" width=3D"100%" border=3D"0" =
cellpadding=3D"0" cellspacing=3D"0"><tbody><tr><td align=3D"center" valign=
=3D"top" class=3D"footer-shell content-padding" style=3D"padding-left: 40px=
; padding-right: 40px; background-color: #ffffff;" bgcolor=3D"#ffffff"><tab=
le width=3D"100%" class=3D"spacer-table" data-testid=3D"spacer" cellpadding=
=3D"0" cellspacing=3D"0"><tbody><tr><td class=3D"spacer" style=3D"font-size=
: 0; line-height: 0; height: 40px;" height=3D"40">=C2=A0</td></tr></tbody><=
/table><table width=3D"100%" cellpadding=3D"0" cellspacing=3D"0"><tbody><tr=
><td valign=3D"top" class=3D"footer-icon-wrapper" style=3D"padding: 0 20px =
0 0;"><table class=3D"component-image image" width=3D"100%" data-testid=3D"=
image" cellpadding=3D"0" cellspacing=3D"0"><tbody><tr><td class=3D"cell com=
ponent-image none" align=3D"center" style=3D"padding-top: 0;"><img src=3D"h=
ttps://assets.nflxext.com/us/email/gem/nflx.png" alt width=3D"24" border=3D=
"0" class=3D"undefined " style=3D"-ms-interpolation-mode: bicubic; border: =
none; outline: none; border-collapse: collapse; display: block;"></td></tr>=
</tbody></table></td><td valign=3D"top" class=3D"footer-copy-wrapper"><tabl=
e class=3D"footer-table" width=3D"100%" valign=3D"top" cellpadding=3D"0" ce=
llspacing=3D"0"><tbody><tr><td class=3D"footer-copy-shell"><table align=3D"=
left" width=3D"100%" class=3D"copy-table footer-copy" data-testid=3D"copy" =
cellpadding=3D"0" cellspacing=3D"0"><tbody><tr><td align=3D"left" class=3D"=
copy p1 none" style=3D"font-family: NetflixSans-Regular, Helvetica, Roboto,=
 Segoe UI, sans-serif; font-weight: 400; font-size: 14px; line-height: 18px=
; letter-spacing: -0.25px; color: #a4a4a4; padding-top: 0;"><span class=3D"=
ignore-diff">=C2=BFPreguntas? Llama al 900-759-106</span></td></tr></tbody>=
</table><table align=3D"left" width=3D"100%" class=3D"copy-table footer-cop=
y address" data-testid=3D"copy" cellpadding=3D"0" cellspacing=3D"0"><tbody>=
<tr><td align=3D"left" class=3D"copy legal none" style=3D"font-family: Netf=
lixSans-Regular, Helvetica, Roboto, Segoe UI, sans-serif; font-weight: 400;=
 font-size: 11px; line-height: 14px; letter-spacing: -0.1px; color: #a4a4a4=
; padding-top: 0;"><span class=3D"hide-link" style=3D"cursor: text; text-de=
coration: none;"><a href=3D"https://help.netflix.com/legal/corpinfo?g=3Dc2d=
d2aad-7647-480a-b786-7810c37e1534&amp;lkid=3DURL_CORP_INFO&amp;lnktrk=3DEVO=
" style=3D"cursor: text; color: #a4a4a4; text-decoration: none;">Netflix Se=
rvicios de Transmisi=C3=B3n Espa=C3=B1a, S.L.</a></span></td></tr></tbody><=
/table><table align=3D"left" width=3D"100%" class=3D"copy-table " data-test=
id=3D"copy" cellpadding=3D"0" cellspacing=3D"0"><tbody><tr><td align=3D"lef=
t" class=3D"copy p2 none" style=3D"font-family: NetflixSans-Regular, Helvet=
ica, Roboto, Segoe UI, sans-serif; font-weight: 400; font-size: 12px; line-=
height: 15px; letter-spacing: -0.12px; padding-top: 20px; color: #a9a6a6;">=
<a class=3D"footer-link" href=3D"https://www.netflix.com/ManageSubscription=
s?g=3Dc2dd2aad-7647-480a-b786-7810c37e1534&amp;lkid=3DURL_COMM_SETTINGS&amp=
;lnktrk=3DEVO&amp;id=3DBQE0AAEBECOicK1LEvsmMBlrZpPOoMSAkL7Ae2xDr5SvB8xuS5GN=
ANognyHYUQiMaNTA4tLYyi3iTvHuvlAk%2BgA7H%2BihDgfLs44dW3S4mcKaFaO0eyW%2Fjr10p=
ukTHT57gJA5joYgQqbDElCz%2FhAS6wf5ZYgF8XTXhNTQYy6Sbrr8DkKgC0P6V5tO4n73%2BJO%=
2Ff2CDdYbpFC1oI4fH9zUrwS%2B2a5pnslc7XA%3D%3D&amp;mid=3Dnone" style=3D"text-=
decoration: underline; line-height: 20px; color: #a4a4a4;">Configuraci=C3=
=B3n de comunicaci=C3=B3n</a><br><a class=3D"footer-link" href=3D"https://w=
ww.netflix.com/TermsOfUse?g=3Dc2dd2aad-7647-480a-b786-7810c37e1534&amp;lkid=
=3DURL_TERMS&amp;lnktrk=3DEVO" style=3D"text-decoration: underline; line-he=
ight: 20px; color: #a4a4a4;">T=C3=A9rminos de uso</a><br><a class=3D"footer=
-link" href=3D"https://www.netflix.com/PrivacyPolicy?g=3Dc2dd2aad-7647-480a=
-b786-7810c37e1534&amp;lkid=3DURL_PRIVACY&amp;lnktrk=3DEVO" style=3D"text-d=
ecoration: underline; line-height: 20px; color: #a4a4a4;">Privacidad</a><br=
><a class=3D"footer-link" href=3D"https://help.netflix.com/help?g=3Dc2dd2aa=
d-7647-480a-b786-7810c37e1534&amp;lkid=3DURL_HELP&amp;lnktrk=3DEVO" style=
=3D"text-decoration: underline; line-height: 20px; color: #a4a4a4;">Centro =
de ayuda</a></td></tr></tbody></table><table align=3D"left" width=3D"100%" =
class=3D"copy-table footer-copy" data-testid=3D"copy" cellpadding=3D"0" cel=
lspacing=3D"0"><tbody><tr><td align=3D"left" class=3D"copy legal none" styl=
e=3D"font-family: NetflixSans-Regular, Helvetica, Roboto, Segoe UI, sans-se=
rif; font-weight: 400; font-size: 11px; line-height: 14px; letter-spacing: =
-0.1px; padding-top: 20px; color: #a4a4a4;">Netflix ha enviado este correo =
a <a href=3D"https://www.netflix.com/browse?g=3Dc2dd2aad-7647-480a-b786-781=
0c37e1534&amp;lkid=3DURL_EMAIL&amp;lnktrk=3DEVO" class=3D"hide-link ignore-=
diff" style=3D"cursor: text; color: #a4a4a4; text-decoration: none;">[albag=
oro98@gmail.com]</a> como parte de tu suscripci=C3=B3n a Netflix.=C2=A0<br>=
SRC: <a href=3D"https://www.netflix.com/browse?g=3Dc2dd2aad-7647-480a-b786-=
7810c37e1534&amp;lkid=3DURL_SRC&amp;lnktrk=3DEVO" class=3D"hide-link ignore=
-diff" style=3D"cursor: text; color: #a4a4a4; text-decoration: none;">61B78=
492_c2dd2aad-7647-480a-b786-7810c37e1534_es-ES_ES_EVO</a></td></tr></tbody>=
</table><table width=3D"100%" class=3D"spacer-table" data-testid=3D"spacer"=
 cellpadding=3D"0" cellspacing=3D"0"><tbody><tr><td class=3D"spacer" style=
=3D"font-size: 0; line-height: 0; height: 40px;" height=3D"40">=C2=A0</td><=
/tr></tbody></table></td></tr></tbody></table></td></tr></tbody></table></t=
d></tr></tbody></table></td></tr></tbody></table></td></tr></tbody></table>=
<div class=3D"mobile-hide-max gmail-fix-no-inline" style=3D"white-space: 'n=
owrap'; font: '15px courier'; line-height: 0;">=C2=A0 =C2=A0 =C2=A0 =C2=A0 =
=C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=
=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0 =
=C2=A0 =C2=A0 =C2=A0 =C2=A0 =C2=A0</div>
    </body>
    </html>
 =20
------=_Part_118186_1531067444.1704905984720--
