## Costing for Azure-S2S-VPN-Setup

To estimate the monthly cost of the Azure setup described, you'll need to consider the pricing for the various resources involved. Here's a breakdown of potential costs:



1. **VPN Gateway**:
   - Azure VPN Gateway pricing depends on the SKU (Basic or VpnGw1, VpnGw2, VpnGw3) and the amount of data transferred. Pricing is based on an hourly rate and varies by region.

2. **Virtual Network (VNet)**:
   - Azure Virtual Network itself does not incur any charges. You pay only for the resources deployed within the VNet.

3. **Subnets**:
   - No additional cost associated with creating subnets within the VNet.

4. **Gateway Subnet**:
   - No additional cost associated with creating a gateway subnet within the VNet.

5. **Public IP Address**:
   - Azure charges for each allocated public IP address. The pricing depends on whether it's a standard or static IP and the region.

6. **Local Network Gateway**:
   - There is no cost to create a local network gateway in Azure. However, outbound data transfer charges may apply if traffic is routed through the gateway.

7. **On-premises VPN**:
   - The cost here would depend on the VPN device or software you're using on-premises. Some software solutions may be free, while others may have licensing fees.

8. **On-premises Public IP Address**:
   - If your on-premises network requires a public IP address for VPN connectivity, there might be costs associated with obtaining and maintaining that IP address from your ISP.

To get an accurate estimate, you would need to check the current pricing for Azure VPN Gateway, public IP addresses, and any potential data transfer costs based on your expected usage. You can use the Azure Pricing Calculator or consult the Azure Pricing documentation for detailed information on pricing for each service. Additionally, it's important to review any potential additional costs related to data transfer, data processing, or other services you may be using in conjunction with your Azure setup.

[Download Excel File](https://github.com/AvinashRode/Azure-S2S-VPN-Setup/blob/main/ExportedEstimate.xlsx)

| Microsoft Azure Estimate |                 |             |                      |                                                                                                                                                  |
| ------------------------ | --------------- | ----------- | -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Your Estimate            |                 |             |                      |                                                                                                                                                  |
| Service category         | Service type    | Custom name | Region               | Description                                                                                                                                      | Estimated monthly cost | Estimated upfront cost |
| Networking               | VPN Gateway     |             | Germany West Central | VPN Gateways, Basic VPN tier, 730 gateway hours, 10 S2S tunnels, 128 P2S connections, 0 GB, VPN outbound VPN gateway type                        | €24.27 | €0.00 |
| Networking               | Virtual Network |             |                      | Germany West Central (Virtual Network 1): 100 GB Outbound Data Transfer; Germany West Central (Virtual Network 2): 100 GB Outbound Data Transfer | €3.69 | €0.00 |
| Networking               | IP Addresses    |             | Germany West Central | Basic (Classic), 1 Dynamic IP Addresses X 730 Hours, 1 Static IP Addresses X 730 Hours                                                           | €2.43 | €0.00 |
| Support                  |                 |             | Support              |                                                                                                                                                  | €0.00 | €0.00 |
|                          |                 |             | Licensing Program    | Microsoft Customer Agreement (MCA)                                                                                                               |  |  |
|                          |                 |             | Billing Account      |                                                                                                                                                  |  |  |
|                          |                 |             | Billing Profile      |                                                                                                                                                  |  |  |
|                          |                 |             | Total                |                                                                                                                                                  | €30.39 | €0.00 |
