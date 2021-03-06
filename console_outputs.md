# Results

Number of unique customers with non-zero revenue :  7204 and the ratio is :  0.011865819390501416

Shape of input datafile: (683145, 60) sampled from 1708337x13 records file

#### Normalising JSON column 'geoNetwork' 
| 0 | {"continent": "Europe", "subContinent": "Western Europe", "country": "Germany", "region": "not available in demo dataset", "metro": "not available in demo dataset", "city": "not available in demo dataset", "cityId": "not available in demo dataset", "networkDomain": "(not set)", "latitude": "not available in demo dataset", "longitude": "not available in demo dataset", "networkLocation": "not available in demo dataset"}                     |
|---|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 | {"continent": "Americas", "subContinent": "Northern America", "country": "United States", "region": "California", "metro": "San Francisco-Oakland-San Jose CA", "city": "Cupertino", "cityId": "not available in demo dataset", "networkDomain": "(not set)", "latitude": "not available in demo dataset", "longitude": "not available in demo dataset", "networkLocation": "not available in demo dataset"}                                              |
| 2 | {"continent": "Americas", "subContinent": "Northern America", "country": "United States", "region": "not available in demo dataset", "metro": "not available in demo dataset", "city": "not available in demo dataset", "cityId": "not available in demo dataset", "networkDomain": "windjammercable.net", "latitude": "not available in demo dataset", "longitude": "not available in demo dataset", "networkLocation": "not available in demo dataset"} |
| 3 | {"continent": "Asia", "subContinent": "Western Asia", "country": "Turkey", "region": "not available in demo dataset", "metro": "not available in demo dataset", "city": "not available in demo dataset", "cityId": "not available in demo dataset", "networkDomain": "unknown.unknown", "latitude": "not available in demo dataset", "longitude": "not available in demo dataset", "networkLocation": "not available in demo dataset"}                    |

|   | geoNetwork.city               | geoNetwork.cityId             | geoNetwork.continent | geoNetwork.country | geoNetwork.latitude           | geoNetwork.longitude          | geoNetwork.metro                  | geoNetwork.networkDomain | geoNetwork.networkLocation    | geoNetwork.region             | geoNetwork.subContinent |
|---|-------------------------------|-------------------------------|----------------------|--------------------|-------------------------------|-------------------------------|-----------------------------------|--------------------------|-------------------------------|-------------------------------|-------------------------|
| 0 | Cupertino                     | not available in demo dataset | Americas             | United States      | not available in demo dataset | not available in demo dataset | San Francisco-Oakland-San Jose CA | (not set)                | not available in demo dataset | California                    | Northern America        |
| 1 | London                        | not available in demo dataset | Europe               | United Kingdom     | not available in demo dataset | not available in demo dataset | London                            | (not set)                | not available in demo dataset | England                       | Northern Europe         |
| 2 | not available in demo dataset | not available in demo dataset | Europe               | Denmark            | not available in demo dataset | not available in demo dataset | not available in demo dataset     | fullrate.ninja           | not available in demo dataset | not available in demo dataset | Northern Europe         |
| 3 | Mexico City                   | not available in demo dataset | Americas             | Mexico             | not available in demo dataset | not available in demo dataset | (not set)                         | uninet-ide.com.mx        | not available in demo dataset | Mexico City                   | Central America         |
| 4 | not available in demo dataset | not available in demo dataset | Europe               | Netherlands        | not available in demo dataset | not available in demo dataset | not available in demo dataset     | (not set)                | not available in demo dataset | not available in demo dataset | Western Europe          |
| 5 | not available in demo dataset | not available in demo dataset | Europe               | United Kingdom     | not available in demo dataset | not available in demo dataset | not available in demo dataset     | unknown.unknown          | not available in demo dataset | not available in demo dataset | Northern Europe         |
| 6 | not available in demo dataset | not available in demo dataset | Europe               | Sweden             | not available in demo dataset | not available in demo dataset | not available in demo dataset     | gavlenet.com             | not available in demo dataset | not available in demo dataset | Northern Europe         |
| 7 | not available in demo dataset | not available in demo dataset | Europe               | United Kingdom     | not available in demo dataset | not available in demo dataset | not available in demo dataset     | virginm.net              | not available in demo dataset | not available in demo dataset | Northern Europe         |
| 8 | not available in demo dataset | not available in demo dataset | Asia                 | India              | not available in demo dataset | not available in demo dataset | not available in demo dataset     | (not set)                | not available in demo dataset | not available in demo dataset | Southern Asia           |
| 9 | not available in demo dataset | not available in demo dataset | Europe               | United Kingdom     | not available in demo dataset | not available in demo dataset | not available in demo dataset     | virginm.net              | not available in demo dataset | not available in demo dataset | Northern Europe         |

	geoNetwork after flattening split into 11 attributes

#### List of all attributes in training set
Index(['Unnamed: 0', 'channelGrouping', 'customDimensions', 'date',
       'fullVisitorId', 'hits', 'socialEngagementType', 'visitId',
       'visitNumber', 'visitStartTime', 'device.browser', 'device.browserSize',
       'device.browserVersion', 'device.deviceCategory', 'device.flashVersion',
       'device.isMobile', 'device.language', 'device.mobileDeviceBranding',
       'device.mobileDeviceInfo', 'device.mobileDeviceMarketingName',
       'device.mobileDeviceModel', 'device.mobileInputSelector',
       'device.operatingSystem', 'device.operatingSystemVersion',
       'device.screenColors', 'device.screenResolution', 'geoNetwork.city',
       'geoNetwork.cityId', 'geoNetwork.continent', 'geoNetwork.country',
       'geoNetwork.latitude', 'geoNetwork.longitude', 'geoNetwork.metro',
       'geoNetwork.networkDomain', 'geoNetwork.networkLocation',
       'geoNetwork.region', 'geoNetwork.subContinent', 'totals.bounces',
       'totals.hits', 'totals.newVisits', 'totals.pageviews',
       'totals.sessionQualityDim', 'totals.timeOnSite',
       'totals.totalTransactionRevenue', 'totals.transactionRevenue',
       'totals.transactions', 'totals.visits', 'trafficSource.adContent',
       'trafficSource.adwordsClickInfo.adNetworkType',
       'trafficSource.adwordsClickInfo.criteriaParameters',
       'trafficSource.adwordsClickInfo.gclId',
       'trafficSource.adwordsClickInfo.isVideoAd',
       'trafficSource.adwordsClickInfo.page',
       'trafficSource.adwordsClickInfo.slot', 'trafficSource.campaign',
       'trafficSource.isTrueDirect', 'trafficSource.keyword',
       'trafficSource.medium', 'trafficSource.referralPath',
       'trafficSource.source'],
      dtype='object')

#### List of constant columns
* socialEngagementType
* device.browserSize 
* device.browserVersion 
* device.flashVersion 
* device.language 
* device.mobileDeviceBranding 
* device.mobileDeviceInfo 
* device.mobileDeviceMarketingName 
* device.mobileDeviceModel 
* device.mobileInputSelector 
* device.operatingSystemVersion 
* device.screenColors 
* device.screenResolution 
* geoNetwork.cityId 
* geoNetwork.latitude 
* geoNetwork.longitude 
* geoNetwork.networkLocation 
* totals.visits 
* trafficSource.adwordsClickInfo.criteriaParameters

Resultant df has now got 41 columns
Shape of Training dataframe after dropping constant columns: (683145, 41)

Shape of Training dataframe after dropping constant columns: (10000, 40)
channelGrouping
device.browser
device.deviceCategory
device.operatingSystem
geoNetwork.city
geoNetwork.continent
geoNetwork.country
geoNetwork.metro
geoNetwork.networkDomain
geoNetwork.region
geoNetwork.subContinent
trafficSource.adContent
trafficSource.adwordsClickInfo.adNetworkType
trafficSource.adwordsClickInfo.gclId
trafficSource.adwordsClickInfo.page
trafficSource.adwordsClickInfo.slot
trafficSource.campaign
trafficSource.keyword
trafficSource.medium
trafficSource.referralPath
trafficSource.source
trafficSource.adwordsClickInfo.isVideoAd
trafficSource.isTrueDirect

Training until validation scores don't improve for 100 rounds.
[100]	valid_0's rmse: 2.03629
[200]	valid_0's rmse: 2.02494
[300]	valid_0's rmse: 2.02037
[400]	valid_0's rmse: 2.01865
Early stopping, best iteration is:
[336]	valid_0's rmse: 2.00881
****************************************************************************************************
Validation Score:
1.928835549344059
Acuuracy Score: 0.825556789
****************************************************************************************************
#### Features List
['channelGrouping', 'fullVisitorId', 'visitStartTime', 'device.browser', 'device.deviceCategory', 
'geoNetwork.networkDomain', 'geoNetwork.continent', 'geoNetwork.country', 'totals.pageviews', 
'totals.timeOnSite', 'totals.transactionRevenue', 'totals.transactions', 'trafficSource.adContent', 'trafficSource.adwordsClickInfo.adNetworkType', 'trafficSource.campaign', 'trafficSource.medium', 'trafficSource.source']
