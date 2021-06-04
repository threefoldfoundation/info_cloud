![](img/tfgrid_pricing.png)

# PROMOTION: Grid Pricing Q1 2021 for TFGrid 2.7 Beta Release

> Prices on testnet are 1/10 of prices mentioned below. 

- pricing is done based on cloud units (see [cloud_units](threefold:cloud_units))

|                   |                                            |              |
| ----------------- | ------------------------------------------ | ------------ |
| Compute Unit (CU) | typically 2 vcpu, 4 GB mem, 50 GB storage  | 80 TFT/month |
| Storage Unit (SU) | typically 1 TB of netto usable storage (*) | 50 TFT/month |
| Network Unit (NU) | 1 GB transfer                              | free for now |

> NOTE: THIS IS A SPECIAL PROMOTION PRICE !!!

> A good site to compare is cloudorado: https://www.cloudorado.com/ <BR>
> TFT price April 12 = 0.12 USD per TFT

(*) if policy of 16+4 and on Harddisk Storage tier

## eVDC Datacenter Pricing 

- Each basic package has
  - 1 kubernetes controller (1GB mem) 
  - 1 ingres network controller (1 IP address) = co-hosted with the kubernetes controller
  - eVDC controller (1GB mem) = your private 3bot for your management of your kubernetes env
  - X chosen CPU capacity (depending chosen package)
  - Y chosen STORAGE capacity

- eVDC starter packages
  - silver: 160 TFT per month for 100GB storage + max 1 CU compute capacity (1 worker)
  - gold: 300 TFT per month for max 2TB storage + max 2 CU compute capacity (1 worker)
  - platinum: 800 TFT per month for max 10TB storage + max 4 CU compute capacity (2 workers)
  
> TODO: prices need to be checked for 2.7 TFGrid

- Additional Capacity (not available testnet)
  - 1 IPv4 address with basic bandwidth: 100 TFT per month
  - CPU & Storage capacity see CU/SU price above.
  - dedicated CPU node (128 GB mem, 48 virtual cpu cores, 500 GB SSD) (BetterToken): 1500 TFT per month, TFGrid 2.8 or TFGrid 2.9

- Each Virtual Datacenter has its own wallet, minimum amount of TFT to start with is the 1 month usage of starting package.
- Billing is done per day = the max resources used in that day.
- The system will warn you if less than 0.5 months of reserve in your own wallet.

## How to get started

see [Get started on TFGrid](threefold:grid_use)