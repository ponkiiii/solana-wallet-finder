# Solana Wallet Hunter: Wallet Discovery and Metrics Tool

## Overview
![image](https://github.com/user-attachments/assets/1c41f262-f50b-4fb5-a915-2dac593f352c)

The **Solana Wallet Hunter** is a robust tool designed to help users discover and analyze wallets interacting with specific Solana tokens. Whether you're tracking token activity, identifying individual traders, or diving into wallet metrics, this tool makes wallet discovery seamless and insightful.

---

## Features

### 🔍 **User Interface**
- **Multi-Token Search**: Enter multiple Solana token addresses to search.
- **Wallet Metrics**: View detailed wallet data:
  - Volume
  - Profit and Loss (PNL)
  - Transaction Count
- **Sorted Results**:
  - Wallets ranked by PNL.
  - Number of tokens matching your search criteria.
- **Interactive Insights**: Click on a wallet to explore its detailed metrics and transaction history.

### 🛠️ **Technical Implementation**
- **Helius API Integration**: Fetches on-chain Solana transaction data.
- **Exchange Filtering**: Removes known exchange wallets to focus on individual trader activity.
- **Data Caching**: Uses PostgreSQL to cache transaction data for faster performance.
- **PNL Analysis**: Calculates profit and loss by analyzing buy/sell transactions.

### 🚀 **Key Features**
- **Multi-Token Search**: Discover wallets interacting with multiple tokens in one query.
- **Exchange Filtering**: Focus on wallets belonging to individual traders, not exchanges.
- **Transaction History**: Complete transaction logs for each wallet.
- **Performance Metrics**: Analyze:
  - Volume traded
  - PNL
  - Token overlap count with your search

---

## How It Works
1. **Enter Token Addresses**: Input Solana token addresses in the search bar.
2. **View Wallets**: See a sorted list of wallets interacting with these tokens.
3. **Explore Metrics**: For each wallet, view its:
   - Total volume
   - PNL
   - Number of transactions
   - Overlap with searched tokens
4. **Interactive Analysis**: Click on a wallet for a detailed breakdown of its transaction history and metrics.

---

## Technical Stack
- **Frontend**: Interactive UI for multi-token searches and wallet analysis.
- **Backend**: 
  - Helius API for on-chain data retrieval.
  - PostgreSQL for caching and performance optimization.
  - PNL calculations based on transaction history.
- **Sorting Logic**: Rank wallets based on:
  - PNL
  - Token overlap count

---

## Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/<your_username>/solana-wallet-hunter.git
   cd solana-wallet-hunter
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Configure your `.env` file:
   - Add your **Helius API Key**.
   - Add your PostgreSQL database credentials.
4. Run the application:
   ```bash
   npm start
   ```
5. Access the tool locally at:
   ```
   http://localhost:3000
   ```

---

## Contributing
Contributions are welcome! Please submit a pull request or open an issue for feedback and feature requests.

## Support
Built by t.me/WaveyHeat
For questions or inquiries, feel free to reach out via the provided link.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

## Acknowledgments
Special thanks to the Solana developer community and the creators of the Helius API for enabling robust blockchain analysis.
