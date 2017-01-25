# PennApps2016

## THSE: The Hacker Sticker Exchange

The Stock Exchange, for your Hackathon Stickers.

**Honorable Mention for the Google Polymer API Prize**

## Components

### Frontend

- `static`: Polymer Frontend

![Screenshot](https://raw.githubusercontent.com/joseph-zhong/PennApps2016/master/stickerexchange.jpg)

### Backend
- `rest.py`: Flask API to connect our Postgresql DB
  - `custom_json_encoder.py`: Custom JSON encoder to handle parsing decimal values
  - `gen_data.py`: Helper function to upsert initial datapoints into Postgresql DB
- `transfers.py`: Helper methods to connect the CapitalOne API 
- `algos.py`: Stock-Exchange related algorithms to handle offer-matching, order enquing and transaction prioritization.
- `bot.py`: Bots to simulate high-frequency trading bots
- `marketprices.py`: Script to update market prices post trades

### Database

- [Entity](https://pennapps2k16.herokuapp.com/entity)
- [Order](https://pennapps2k16.herokuapp.com/order/)
- [Ledger](https://pennapps2k16.herokuapp.com/ledger/)
- [Priority Queue](https://pennapps2k16.herokuapp.com/priority_queue/)
- [Inventory](https://pennapps2k16.herokuapp.com/inventory/)
- [Price History](https://pennapps2k16.herokuapp.com/price_history/<string:ticker>)

