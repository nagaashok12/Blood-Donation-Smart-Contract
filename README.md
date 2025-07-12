# 🩸 Blood Donation Smart Contract

A decentralized application (dApp) built with Solidity that enables hospitals to manage patient registrations and track blood donation or reception transactions securely on the Ethereum blockchain.

---

## ⚙️ Features

- ✅ Register hospitals with name, contact, location, and fees
- ✅ Register patients with name, age, blood group, contact, and Aadhar
- ✅ Record blood transactions (donor or receiver)
- ✅ Access full or individual patient records using Aadhar
- ✅ Owner-only access control for sensitive functions

---

## 🛠 Tech Stack

- **Solidity** (Smart Contract Language)
- **Ethereum** Blockchain


## 🔐 Access Control

Only the contract `owner` (deployer address) can:
- Add hospitals
- View all patient records
- Record blood transactions

Patients can:
- Register themselves using their Aadhar

---

## 📦 Smart Contract Structure

### 🏥 HospitalDetails

```solidity
struct HospitalDetails {
    string name;
    uint contact;
    string location;
    uint fees;
}
