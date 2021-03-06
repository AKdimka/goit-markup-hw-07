# AKdimka-goit-markup-hw-07

a,
a:visited {
	text-decoration: none;
}
h1,
h2,
h3,
p {
	margin: 0;
}
ul {
	list-style: none;
	margin: 0;
	padding: 0;
}
img {
	display: block;
	max-width: 100%;
	height: auto;
}
:root {
	--brand-color: #2196f3;
	--btn-second: #188ce8;
	--primery-text-color: #757575;
	--secondary-text-color: #212121;
	--bg-color: #ffffff;
	--secondary-bg: #2f303a;
	--third-bg: #f5f4fa;
	--item-gap: 30px;
}
body {
	font-family: "Roboto", sans-serif;
	letter-spacing: 0.03em;
	color: var(--primery-text-color);
	font-size: 14px;
}
.container {
	width: 1200px;
	padding-left: 15px;
	padding-right: 15px;

	margin-left: auto;
	margin-right: auto;
}
.section {
	padding-top: 94px;
	padding-bottom: 94px;
}
.link:hover,
.link:focus {
	color: var(--brand-color);
	fill: var(--brand-color);
}
.btn:hover,
.btn:focus {
	background-color: var(--btn-second);
}
/* -------Хедер------- */
.header {
	display: flex;
	align-items: center;
	justify-content: space-between;

	background: var(--bg-color);
	border-bottom: 1px solid #ececec;
}
.logo {
	font-family: "Raleway", sans-serif;
	font-weight: 700;
	font-size: 26px;
	line-height: 1.19;
	color: var(--secondary-text-color);
}
.logo-1 {
	color: var(--brand-color);
}
.header-nav {
	display: flex;
	align-items: center;
}
.header-nav__list {
	display: flex;
	margin-left: 93px;
}
.nav-list {
}
.nav-list__item:not(:first-child) {
	margin-left: 50px;
}
.nav-list__link {
	position: relative;
	display: block;
	font-weight: 500;
	line-height: 1.14;
	letter-spacing: 0.02em;

	padding-top: 32px;
	padding-bottom: 32px;

	transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1), fill 250ms cubic-bezier(0.4, 0, 0.2, 1);
	color: var(--secondary-text-color);
}
.nav-list__link--current {
	color: var(--brand-color);
}
.nav-list__link--current::after {
	content: "";

	position: absolute;
	left: 0;
	bottom: 0;

	display: block;
	width: 100%;
	height: 4px;
	border-radius: 2px;

	background: var(--brand-color);
}
.header__contacts {
	display: flex;
	align-items: center;
}
.header-contacts-list__item:not(:first-child) {
	margin-left: 50px;
}
.header-contacts-list__icon {
	fill: currentColor;
	margin-right: 10px;
}
.header-contacts-list__link {
	display: flex;
	align-items: center;
	font-weight: 500;
	line-height: 1.14;
	letter-spacing: 0.02em;

	transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1), fill 250ms cubic-bezier(0.4, 0, 0.2, 1);
	color: var(--primery-text-color);
}
/* -------Герой------- */
.hero {
	text-align: center;
	padding-top: 200px;
	padding-bottom: 200px;

	background-color: var(--secondary-bg);
	background-image: linear-gradient(to right, rgba(47, 48, 58, 0.4), rgba(47, 48, 58, 0.4)), url(../images/bg/bg.jpg);
	background-repeat: no-repeat;
	background-position: center;
	background-size: cover;
}
.hero__title {
	font-weight: 900;
	font-size: 44px;
	line-height: 1.36;
	width: 700px;

	margin-right: auto;
	margin-left: auto;

	letter-spacing: 0.06em;
	text-transform: uppercase;

	color: var(--bg-color);
}
.btn {
	cursor: pointer;
	font-family: "roboto", sans-serif;
	font-weight: 700;
	font-size: 16px;
	line-height: 1.9;
	letter-spacing: 0.06em;

	padding: 10px 32px;
	border: 0px;

	color: var(--bg-color);

	background-color: var(--brand-color);
	box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.15);
	border-radius: 4px;
	transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.hero__button {
	margin-top: 30px;
}
/* ------- Backdrop ------- */
.backdrop {
	position: fixed;
	top: 0;
	left: 0;
	width: 100vw;
	height: 100vh;
	opacity: 1;

	transition: opacity 250ms cubic-bezier(0.4, 0, 0.2, 1);

	background: rgba(0, 0, 0, 0.2);
}
.backdrop.is-hidden {
	opacity: 0;
	pointer-events: none;
}

/* ------- Modal ------- */
.backdrop__modal {
	position: absolute;
	top: 50%;
	left: 50%;
	max-width: 528px;
	transform: translate(-50%, -50%);

	padding: 40px;
	box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.12), 0px 1px 1px rgba(0, 0, 0, 0.14), 0px 2px 1px rgba(0, 0, 0, 0.2);
	border-radius: 4px;
	background: #fff;
}
.modal {
}
.modal__close-btn {
	position: fixed;
	top: 8px;
	right: 8px;
	width: 30px;
	height: 30px;

	display: flex;
	align-items: center;
	justify-content: center;

	cursor: pointer;
	background: #ffffff;
	border: 1px solid rgba(0, 0, 0, 0.1);
	border-radius: 50%;
}
.modal__close-btn:hover,
.modal__close-btn:focus {
	fill: var(--brand-color);
}
.modal__title {
	font-size: 20px;
	line-height: 23px;

	color: var(--secondary-text-color);
}
.modal__form {
	margin-top: 12px;
}
.form {
}
.form__field {
	position: relative;
	display: flex;
	flex-direction: column;
	align-items: flex-start;

	font-family: "Roboto";
	font-size: 12px;
	line-height: 1.16;
	letter-spacing: 0.01em;
}
.form__field:not(:first-child) {
	margin-top: 10px;
}
.form__input {
	width: 100%;
	margin-top: 4px;
	resize: none;

	padding: 11px 12px 11px 35px;

	border: 1px solid rgba(33, 33, 33, 0.2);
	border-radius: 4px;
	transition: border 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.form__input-svg {
	position: absolute;
	top: 27px;
	left: 12px;
	transition: fill 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.form__input:focus {
	border: 1px solid var(--brand-color);
	outline: none;
}
.form__input:focus + .form__input-svg {
	fill: var(--brand-color);
}
.form__input--comment {
	padding: 12px 16px;
}
.form__policy {
	display: flex;
	margin-top: 20px;
}
.policy {
}
.policy__checkbox {
	position: absolute;
	width: 1px;
	height: 1px;
	margin: -1px;
	border: 0;
	padding: 0;
	clip: rect(0 0 0 0);
	overflow: hidden;
}
.policy__checkbox:hover + .policy__icon,
.policy__checkbox:focus + .policy__icon {
	border-color: var(--brand-color);
}
.policy__icon {
	display: inline-block;
	margin-right: 8px;
	width: 16px;
	height: 15px;
	border: 2px solid var(--secondary-text-color);
	border-radius: 2px;
	transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1), border-color 250ms cubic-bezier(0.4, 0, 0.2, 1),
		background-image 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.policy__checkbox:checked + .policy__icon {
	border-color: var(--brand-color);
	background-color: var(--brand-color);
	background-image: url(../images/icon-check.svg);
	background-size: contain;
	background-origin: border-box;
}
.policy__link {
	color: var(--brand-color);
	text-decoration: underline;
	transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.policy__link:hover,
.policy__link:focus {
	color: var(--btn-second);
	text-decoration: none;
}
.form__submit-btn {
	display: block;
	margin-top: 30px;
	margin-left: auto;
	margin-right: auto;
}
/* -------Особенности------- */
.features {
}
.visibility-hiden {
	position: absolute;
	width: 1px;
	height: 1px;
	margin: -1px;
	border: 0;
	padding: 0;
	clip: rect(0 0 0 0);
	overflow: hidden;
}
.features-list {
	display: flex;
}
.features__item {
	width: calc((100% - 90px) / 4);
}
.features__thumb {
	display: flex;
	justify-content: center;
	padding: 25px 0;
	background: var(--third-bg);
	border-radius: 4px;
}
.features__svg {
}
.features__item:not(:first-child) {
	margin-left: var(--item-gap);
}
.features__item-title {
	font-weight: 700;
	font-size: 14px;
	line-height: 1.14;
	text-transform: uppercase;

	margin-top: 30px;

	color: var(--secondary-text-color);
}
.features__description {
	font-weight: 400;
	font-size: 14px;
	line-height: 1.7;

	margin-top: 10px;
}

/* -------Чем мы занимаемся------- */
.skill-section {
	padding-top: 0;
}
.skill-section__title {
	font-weight: 700;
	font-size: 36px;
	line-height: 1.16;
	text-align: center;

	color: var(--secondary-text-color);
}
.skill-section__list {
	display: flex;
	margin-top: 50px;
}
.skill-section__item {
	position: relative;
}
.skill-section__item:not(:first-child) {
	margin-left: var(--item-gap);
}
.skill-section__img {
}
.skill-section__label {
	position: absolute;
	bottom: 0;
	width: 100%;
	padding: 27px 0;
	background: rgba(47, 48, 58, 0.8);
}
.skill-section__name {
	font-weight: 700;
	font-size: 14px;
	line-height: 16px;
	text-align: center;
	letter-spacing: 0.03em;
	text-transform: uppercase;

	color: var(--bg-color);
}

/* -------Наша команда------- */
.workers-section {
	background: var(--third-bg);
	text-align: center;
}
.workers-section__title {
	font-weight: 700;
	font-size: 36px;
	line-height: 1.16;

	color: var(--secondary-text-color);
}
.workers-section__list {
	display: flex;
	margin-top: 50px;
}
.workers {
}
.workers__card:not(:first-child) {
	margin-left: var(--item-gap);
}
.workers__card {
	box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.12), 0px 1px 1px rgba(0, 0, 0, 0.14), 0px 2px 1px rgba(0, 0, 0, 0.2);
	border-radius: 0px 0px 4px 4px;

	overflow: hidden;
}
.workers-card__content {
	padding-top: 30px;
	padding-bottom: 30px;

	background-color: var(--bg-color);
}
.workers-card__name {
	font-weight: 500;
	font-size: 16px;
	line-height: 1.2;

	color: var(--secondary-text-color);
}
.workers-card__position {
	font-weight: 400;
	font-size: 16px;
	line-height: 1.19;

	margin-top: 10px;
}
.workers-card__media {
	display: flex;
	margin-top: 16px;
	justify-content: center;
}
.card-media__item:not(:first-child) {
	margin-left: 10px;
}
.card-media__item {
}
.card-media__link {
	display: flex;
	align-items: center;
	justify-content: center;
	height: 44px;
	width: 44px;
	border-radius: 50%;

	fill: #afb1b8;

	transition: fill 250ms cubic-bezier(0.4, 0, 0.2, 1), background-color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.card-media__link:focus,
.card-media__link:hover {
	fill: var(--bg-color);
	background-color: var(--brand-color);
}
.icon {
	height: 20px;
	width: 20px;
}
/* -------Наши клиенты------- */
.client-section {
}
.client-section__title {
	font-weight: 700;
	font-size: 36px;
	line-height: 1.16;
	text-align: center;

	color: var(--secondary-text-color);
}
.client-section__list {
	display: flex;
	margin-top: 50px;
}
.client-section__item:not(:first-child) {
	margin-left: var(--item-gap);
}
.client-section__link {
	display: block;

	padding: 16px 32px;

	fill: #afb1b8;
	border: 1px solid #afb1b8;
	border-radius: 4px;

	transition: fill 250ms cubic-bezier(0.4, 0, 0.2, 1), border-color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.client-section__link:focus,
.client-section__link:hover {
	fill: var(--brand-color);
	border-color: var(--brand-color);
}
.client-section__logo {
}

/* -------Подвал------- */
.footer-section {
	padding-top: 60px;
	padding-bottom: 60px;
	background-color: var(--secondary-bg);
}
.footer-section__container {
	display: flex;
	align-items: baseline;
}
.footer-section__contacts {
}
.logo--contrast {
	color: var(--bg-color);
}
.footer-contacts__address {
	margin-top: 20px;
}
.footer-contacts__item:not(:first-child) {
	margin-top: 9px;
}
.footer-contacts__link {
	font-style: normal;
	font-weight: 400;
	font-size: 14px;
	line-height: 1.7;

	color: rgba(255, 255, 255, 0.6);
	transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.footer-contacts__link--street {
	color: var(--bg-color);
}

.footer-section__join-box {
	margin-left: 70px;
}
.join-box {
}
.join-box__title {
	font-weight: 700;
	font-size: 14px;
	line-height: 16px;
	text-transform: uppercase;

	color: var(--bg-color);
}
.join-box__list {
	display: flex;
	margin-top: 20px;
}
.join-box__item:not(:first-child) {
	margin-left: 10px;
}
.join-box__link {
	display: block;
	height: 44px;
	width: 44px;
	border-radius: 50%;

	padding: 12px;
	fill: var(--bg-color);
	background: rgba(255, 255, 255, 0.1);

	transition: background 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.join-box__link:hover,
.join-box__link:focus {
	background: var(--brand-color);
}

.footer-section__subscribe-box {
	margin-left: 70px;
}
.subscribe-box {
}
.subscribe-box__title {
	font-style: normal;
	font-size: 14px;
	text-transform: uppercase;

	color: var(--bg-color);
}
.subscribe-box__form {
	display: flex;
	margin-top: 20px;
	flex-direction: row;
	align-items: baseline;
}
.subscribe-box__input {
	width: 358px;
	padding: 15px 16px;

	background: inherit;
	border: 1px solid rgba(255, 255, 255, 0.3);
	filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.15));
	border-radius: 4px;
}
.subscribe-box__btn {
	display: flex;
	margin-left: 12px;
}
.subscribe-box__btn-svg {
	margin-left: 10px;
}
/* --------------Портфолио-------------- */
/* -------Фильтр------- */
.filter {
	display: flex;
	justify-content: center;

	margin-bottom: 50px;
}
.filter__item:not(:first-child) {
	margin-left: 8px;
}
.filter__button {
	cursor: pointer;
	font-family: "Roboto", sans-serif;
	font-weight: 500;
	font-size: 16px;
	line-height: 1.6;

	padding-top: 6px;
	padding-bottom: 6px;
	padding-right: 22px;
	padding-left: 22px;

	text-align: center;
	color: var(--secondary-text-color);
	border: transparent;

	background: var(--third-bg);
	border-radius: 4px;

	transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1), background 250ms cubic-bezier(0.4, 0, 0.2, 1),
		box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.filter__button:hover,
.filter__button:focus {
	color: var(--bg-color);
	background: var(--brand-color);

	box-shadow: 0px 3px 1px rgba(0, 0, 0, 0.1), 0px 1px 2px rgba(0, 0, 0, 0.08), 0px 2px 2px rgba(0, 0, 0, 0.12);
}

/* -------Проэкты------- */
.projects-section {
	display: flex;
	flex-wrap: wrap;

	margin-top: calc(-1 * var(--item-gap));
	margin-left: calc(-1 * var(--item-gap));
}
.projects-section__item {
	margin-top: var(--item-gap);
	margin-left: var(--item-gap);

	flex-basis: calc((100% - var(--item-gap) * 3) / 3);
}
.project-card {
}
.project-card__link {
	display: block;

	transition: box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.project-card__link:focus,
.project-card__link:hover {
	box-shadow: 0px 1px 1px rgba(0, 0, 0, 0.12), 0px 4px 4px rgba(0, 0, 0, 0.06), 1px 4px 6px rgba(0, 0, 0, 0.16);
}
.project-card__thumb {
	position: relative;
	overflow: hidden;
}
.project-card__content {
	padding-top: 20px;
	padding-bottom: 20px;
	padding-left: 24px;
	padding-right: 24px;

	border-left: 1px solid #eeeeee;
	border-bottom: 1px solid #eeeeee;
	border-right: 1px solid #eeeeee;
}
.project-card__name {
	font-weight: 700;
	font-size: 18px;
	line-height: 2;

	letter-spacing: 0.06em;

	color: var(--secondary-text-color);
}
.project-card__text {
	font-weight: 400;
	font-size: 16px;
	line-height: 1.9;

	color: var(--primery-text-color);
}
.project-card__description {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	font-size: 18px;
	line-height: 1.56;

	padding: 63px 24px;

	background: rgba(33, 150, 243, 0.9);
	transition: transform 250ms cubic-bezier(0.4, 0, 0.2, 1);
	transform: translateY(101%);

	color: #fff;
}
.project-card__link:hover .project-card__description,
.project-card__link:focus .project-card__description {
	transform: translateY(0);
}
