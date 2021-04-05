![](img/tfgrid_pricing.png)

# PROMOTION: Grid Pricing Q1 2021 for DIY capacity

> Prices on testnet are 1/10 of prices mentioned below. 

- DIY = Do It Yourself Capacity
- pricing is done based on cloud units (see [cloud_units](threefold:cloud_units))

|                   |                                            |              |
| ----------------- | ------------------------------------------ | ------------ |
| Compute Unit (CU) | typically 2 vcpu, 4 GB mem, 50 GB storage  | 10 USD/month |
| Storage Unit (SU) | typically 1 TB of netto usable storage (*) | 8 USD/month  |
| Network Unit (NU) | 1 GB transfer                              | free for now |

> A good site to compare is cloudorado: https://www.cloudorado.com/

(*) if policy of 16+4 and on Harddisk Storage tier

## Virtual Planetary Scale Datacenter Pricing 

- Each basic package has
  - 1 kubernetes controller (1GB mem) 
  - 1 ingres network controller (1 IP address) = co-hosted with the kubernetes controller
  - eVDC controller (1GB mem) = your private 3bot for your management of your kubernetes env
  - X chosen CPU capacity (depending chosen package)
  - Y chosen STORAGE capacity

- eVDC starter packages
  - silver: 15 USD per month for 100GB storage + max 1 CU compute capacity (1 worker)
  - gold: 30 USD per month for max 2TB storage + max 2 CU compute capacity (1 worker)
  - platinum: 80 USD per month for max 10TB storage + max 4 CU compute capacity (2 workers)
  

- Additional Capacity (not available testnet)
  - 1 IP address with basic bandwidth: 1-5 EUR per month (depends on farmer)
  - dedicated CPU node (128 GB mem, 48 virtual cpu cores, 500 GB SSD) (BetterToken)
  - CPU & Storage capacity, see pricing as done by farmers, typicall around 10-15 USD per CU, and 5 to 10 USD per SU.


- Each Virtual Datacenter has its own wallet, minimum amount of TFT to start with is the 1 month usage of starting package.
- Billing is done per day = the max resources used in that day.
- The system will warn you if less than 0.5 months of reserve in your own wallet.

## How to get started

see [Get started on TFGrid](threefold:use_tfgrid)