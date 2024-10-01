OpenRTB (Open Real-Time Bidding) is a protocol that standardizes the way advertisers and publishers communicate during the programmatic advertising process. The protocol outlines how bid requests and responses are formatted, ensuring compatibility across different platforms and systems.

### Key Components of OpenRTB

1. **Bid Request**: This is a JSON object sent from the publisher's ad server to potential bidders (advertisers). It includes information such as:
   - **ID**: Unique identifier for the bid request.
   - **Impression**: Details about the ad space (size, type, etc.).
   - **Site/App**: Information about the website or app where the ad will be displayed.
   - **User**: Data related to the user (if available), such as demographics, interests, etc.
   - **Device**: Information about the device being used (OS, browser, etc.).
   - **Price Floor**: Minimum price the publisher is willing to accept.

2. **Bid Response**: After receiving a bid request, advertisers respond with a bid response, which includes:
   - **ID**: Unique identifier that matches the bid request.
   - **Seat Bid**: Contains one or more bid objects, each detailing:
     - **Bid ID**: Unique identifier for the bid.
     - **Impression ID**: The ID of the impression being bid on.
     - **Price**: The bid amount.
     - **Ad ID**: Identifier for the ad being offered.
     - **Creative**: The ad content, which can be a URL to the ad asset.

3. **Winning Bid Notification**: If an advertiser wins the auction, the system notifies the ad server, which then serves the ad to the user.

### Example JSON Structure

**Bid Request Example:**

```json
{
  "id": "123456789",
  "imp": [{
    "id": "1",
    "banner": {
      "w": 300,
      "h": 250
    },
    "bidfloor": 0.50
  }],
  "site": {
    "id": "987",
    "name": "example.com",
    "domain": "example.com"
  },
  "user": {
    "id": "user123",
    "keywords": "sports, music"
  },
  "device": {
    "ip": "192.0.2.1",
    "ua": "Mozilla/5.0"
  }
}
```

**Bid Response Example:**

```json
{
  "id": "123456789",
  "seatbid": [{
    "seat": "advertiser1",
    "bid": [{
      "id": "bid1",
      "impid": "1",
      "price": 1.50,
      "adm": "<html>Ad content here</html>"
    }]
  }]
}
```

### Versioning

OpenRTB has several versions (e.g., 2.3, 2.4, 2.5) that introduce new fields and updates. It's important to refer to the official OpenRTB specification for the version you are using, as the structure and available fields may vary.

### Conclusion

OpenRTB facilitates seamless and efficient communication between publishers and advertisers, enabling real-time bidding for digital ad inventory. By adhering to the protocol, companies can ensure that their systems work well together in the dynamic landscape of programmatic advertising.


----------------------------------------------------------------------------------------------------------------
Programmatic ad’s means it is a process of automatic buying advertising space on websites and Apps. Programmatic advertising makes it is possibilities purchase and ad place including targeting advertising content in less than one second.
The Ad’s are placed through the system known as RTB (real time bidding). It’s manage transaction between publisher side (supply side) and advertise side (demand side).
![Screenshot 2024-09-29 at 23 34 58](https://github.com/user-attachments/assets/1ed79871-8518-4af5-9e8f-4d6944207a21)
![Screenshot 2024-09-29 at 23 35 35](https://github.com/user-attachments/assets/e47b8bbf-e1d1-4784-a9bb-29d5bfb621fa)
Real Time Bidding - It enables the buying and selling of digital advertising through auctions which take place in a time-frame of milliseconds.
![Screenshot 2024-09-29 at 23 51 24](https://github.com/user-attachments/assets/233c6c2a-4795-4026-ba4d-701e2b6865cc)
![Screenshot 2024-09-30 at 11 28 34](https://github.com/user-attachments/assets/2d99d386-880e-495c-b8d4-2e367d3ef2d5)
![Screenshot 2024-09-30 at 11 32 51](https://github.com/user-attachments/assets/3de0f439-8c74-475a-bf06-d35576b41511)
Demand Side Platform - It is an advertising technology platform used by #advertisers and #agencies to automate the purchase of advertising.
![Screenshot 2024-09-30 at 11 50 50](https://github.com/user-attachments/assets/36e40375-e924-4681-b4ba-dc066675a7ce)
![Screenshot 2024-09-30 at 11 52 58](https://github.com/user-attachments/assets/e5e5bac6-51af-4863-9a30-9291a04bb029)
![Screenshot 2024-09-30 at 17 41 42](https://github.com/user-attachments/assets/a39d54d8-1409-4600-bb6b-a6795edd8e36)
![Screenshot 2024-09-30 at 17 42 08](https://github.com/user-attachments/assets/44929d5c-17ef-48cd-87c0-6238350ae9fd)
Supply Side Platform - It is an advertising technology platform used by #publishers to manage, sell and optimize available inventory (ad space) on their websites and mobile apps in an automated and efficient way.
![Screenshot 2024-09-30 at 17 45 53](https://github.com/user-attachments/assets/8177dfe9-5988-4dc7-97ce-9d0f1f5f4e89)
![Screenshot 2024-09-30 at 17 47 50](https://github.com/user-attachments/assets/37573a0a-a069-407f-b723-e09f4dde4a90)
![Screenshot 2024-09-30 at 17 52 45](https://github.com/user-attachments/assets/7d64813f-66d3-4ad6-a551-ff1944df0161)
brand safety, dont show my ads on shady places
![Screenshot 2024-09-30 at 17 55 43](https://github.com/user-attachments/assets/a4efe67c-17ac-4ad8-b4bb-a09a1db348a9)
![Screenshot 2024-09-30 at 17 58 47](https://github.com/user-attachments/assets/51b5970a-d226-4520-a78a-0358221af5b1)
An Ad Exchange is where publishers meet advertisers and agree on a price to display their ads. The ad exchange sits in the middle of the programmatic ecosystem and is plugged into a Demand-Side Platform (DSP) on the advertiser's side and a Supply-Side Platform (SSP) on the publisher's side.
![Screenshot 2024-09-30 at 18 00 32](https://github.com/user-attachments/assets/a3cfc092-1e38-439a-857c-fe976bc88661)
![Screenshot 2024-09-30 at 18 08 27](https://github.com/user-attachments/assets/08bca883-aea3-4c8e-9f40-461cd4a81dfa)
Ad Network -- A business that sells ad space on behalf of multiple publishers.
![Screenshot 2024-09-30 at 18 11 00](https://github.com/user-attachments/assets/ba458496-51a3-4971-87c5-c406cd203ea9)
![Screenshot 2024-09-30 at 20 34 04](https://github.com/user-attachments/assets/774e5050-26ce-4345-ab03-95e7c3762451)
![Screenshot 2024-09-30 at 20 34 59](https://github.com/user-attachments/assets/4ac02bb3-2d70-4da6-9e53-46781fc65988)
![Screenshot 2024-09-30 at 20 35 49](https://github.com/user-attachments/assets/ca7794de-0a02-4b37-a6a8-138ec506fb30)
![Screenshot 2024-09-30 at 20 36 51](https://github.com/user-attachments/assets/54e959a5-8a1e-4335-a70d-e9f3b93bfdb2)
Ad Exchange  -- An Ad Exchange is where publishers meet advertisers and agree on a price to display their ads. The ad exchange sits in the middle of the programmatic ecosystem and is plugged into a Demand-Side Platform (DSP) on the advertiser's side and a Supply-Side Platform (SSP) on the publisher's side.
![Screenshot 2024-09-30 at 20 38 57](https://github.com/user-attachments/assets/90bed749-aaee-475b-b20c-753c0b4c0aa2)
