# Архитектура PUSH уведомлений

## Поток
Mobile App → API Gateway → Notification Service → Message Broker → Firebase/APNS → Device

## Источники событий
- Cart Service — брошенная корзина
- Order Service — статус заказа
- Marketing Service — рекламные рассылки

## Причины использования брокера
- асинхронная обработка
- повторные отправки
- массовые рассылки
- отказоустойчивость
