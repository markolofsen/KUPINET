![Best API for Binance 2018](https://github.com/Kupinet/storage/raw/master/logo_banners/binance.jpg)

# Best API for Binance 2018

Nice library for Binance

[Check out the Interactive Demo](http://kupi.net/p/docs-api)

> Благодаря этому модулю вы сможете разрабатывать собственных крипто-ботов, анализировать крипто-рынки и конечно, зарабатывать деньги.
>
> Our web-service works 24 hours and keeps high loads
>
> Данные всех бирж приходят в едином формате и содержат расширенную информацию (ссылки для перехода на торговые пары, лучшие аски и биды, курсы валют и многое другое).
>
> - Бесплатно!
> - Актуальность ордеров 5—30 секунд!
> - Данные со большинства бирж
> - Круглосуточная поддержка



### Installation Instructions
    $ pip3 install KUPINET

### Init example
```python
from KUPINET import KUPI

# Specify free api key like global variable
KUPINET_API_KEY = 'freeApi'
```

### Stocks API
```python
# Get all stocks
KUPI.NET.Stocks().getList()

# Get orders by Stock name
KUPI.NET.Stocks('Binance').getOrders('ETH','BTC')

# Get all pairs from the Stock
KUPI.NET.Stocks('Binance').getAllPairs()
```
### Pairs API
```python
# Find best prices for Pair in all Stocks
KUPI.NET.Pair('LTC','ETH').getBestPrices()
```
### Find Best Prices API
```python
# Find best ASK
KUPI.NET.BestPrices('LTC').Ask()

# Find best BID
KUPI.NET.BestPrices('LTC').Bid()
```
### Cryptocurrency Converter (Calculator) API
```python
# Coins list
KUPI.NET.Calc().Data()

# Convert Coin to Coin
KUPI.NET.Calc('LTC','ETH').Amount(10)
```

## Roadmap
- Выгрузка исторических данных по торговле
- Мультри-трейдинг через единый терминал
- Инструмент для крипто-арбитража
- API для JavaScript, PHP, C#
- Запуск децентрализованной биржи
- Виджет (калькулятор) для интеграции с сайтами


## Abouts us
> We are a team of crypto developers. Our goal is to make the most convenient crypto services possible.
[Contact with us](http://kupi.net/p/support)