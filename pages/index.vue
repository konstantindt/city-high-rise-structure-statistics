
<template>
  <div>
    <v-data-table
      :headers='headers'
      :items='cityViews'
      :items-per-page='37'
      :light='true'
      caption='City high-rise structure statistics'
      class='elevation-1'
    >
      <template v-slot:header>
        <thead>
          <tr>
            <th :colspan='4' />
            <th :colspan='4' class='join-header' style='text-align: center'>
              Buildings with height
            </th>
            <th :colspan='2' />
          </tr>
        </thead>
      </template>
    </v-data-table>
  </div>
</template>

<script>
export default {
  data () {
    return {
      headers: [
        {
          text: '#',
          align: 'left',
          sortable: false,
          value: '#'
        },
        { text: 'City', value: 'City' },
        { text: 'Country', value: 'Country' },
        { text: 'All buildings', value: 'All Buildings' },
        { text: '> 100m', value: '100m+' },
        { text: '> 150m', value: '150m+' },
        { text: '> 200m', value: '200m+' },
        { text: '> 300m', value: '300m+' },
        { text: 'Telecom towers', value: 'Telecom Towers' },
        { text: 'All structures', value: 'All Structures' }
      ],
      cityViews: [
        {
          '#': 2,
          'City': 'New York City',
          'Country': 'United States',
          'All Buildings': 1390,
          '100m+': 803,
          '150m+': 257,
          '200m+': 66,
          '300m+': 7,
          'Telecom Towers': 2,
          'All Structures': 1398
        },
        {
          '#': 1,
          'City': 'Hong Kong',
          'Country': 'China',
          'All Buildings': 820,
          '100m+': 555,
          '150m+': 317,
          '200m+': 64,
          '300m+': 6,
          'Telecom Towers': 0,
          'All Structures': 820
        },
        {
          '#': 6,
          'City': 'Chicago',
          'Country': 'United States',
          'All Buildings': 524,
          '100m+': 317,
          '150m+': 119,
          '200m+': 29,
          '300m+': 6,
          'Telecom Towers': 1,
          'All Structures': 526
        },
        {
          '#': 4,
          'City': 'Tokyo',
          'Country': 'Japan',
          'All Buildings': 348,
          '100m+': 284,
          '150m+': 145,
          '200m+': 26,
          '300m+': 0,
          'Telecom Towers': 2,
          'All Structures': 351
        },
        {
          '#': 3,
          'City': 'Dubai',
          'Country': 'United Arab Emirates',
          'All Buildings': 370,
          '100m+': 266,
          '150m+': 176,
          '200m+': 68,
          '300m+': 20,
          'Telecom Towers': 0,
          'All Structures': 370
        },
        {
          '#': 17,
          'City': 'Toronto',
          'Country': 'Canada',
          'All Buildings': 487,
          '100m+': 241,
          '150m+': 54,
          '200m+': 18,
          '300m+': 0,
          'Telecom Towers': 1,
          'All Structures': 489
        },
        {
          '#': 5,
          'City': 'Shanghai',
          'Country': 'China',
          'All Buildings': 379,
          '100m+': 183,
          '150m+': 141,
          '200m+': 52,
          '300m+': 5,
          'Telecom Towers': 2,
          'All Structures': 381
        },
        {
          '#': 29,
          'City': 'Moscow',
          'Country': 'Russia',
          'All Buildings': 204,
          '100m+': 165,
          '150m+': 37,
          '200m+': 15,
          '300m+': 5,
          'Telecom Towers': 3,
          'All Structures': 207
        },
        {
          '#': 11,
          'City': 'Seoul',
          'Country': 'South Korea',
          'All Buildings': 158,
          '100m+': 138,
          '150m+': 82,
          '200m+': 18,
          '300m+': 1,
          'Telecom Towers': 1,
          'All Structures': 159
        },
        {
          '#': 8,
          'City': 'Chongqing',
          'Country': 'China',
          'All Buildings': 146,
          '100m+': 136,
          '150m+': 110,
          '200m+': 35,
          '300m+': 2,
          'Telecom Towers': 0,
          'All Structures': 146
        },
        {
          '#': 10,
          'City': 'Singapore',
          'Country': 'Singapore',
          'All Buildings': 203,
          '100m+': 129,
          '150m+': 84,
          '200m+': 32,
          '300m+': 0,
          'Telecom Towers': 1,
          'All Structures': 204
        },
        {
          '#': 13,
          'City': 'Jakarta',
          'Country': 'Indonesia',
          'All Buildings': 382,
          '100m+': 128,
          '150m+': 74,
          '200m+': 33,
          '300m+': 0,
          'Telecom Towers': 2,
          'All Structures': 383
        },
        {
          '#': 7,
          'City': 'Shenzhen',
          'Country': 'China',
          'All Buildings': 145,
          '100m+': 125,
          '150m+': 114,
          '200m+': 58,
          '300m+': 8,
          'Telecom Towers': 0,
          'All Structures': 145
        },
        {
          '#': 9,
          'City': 'Guangzhou',
          'Country': 'China',
          'All Buildings': 161,
          '100m+': 125,
          '150m+': 103,
          '200m+': 30,
          '300m+': 9,
          'Telecom Towers': 1,
          'All Structures': 163
        },
        {
          '#': 33,
          'City': 'Sydney',
          'Country': 'Australia',
          'All Buildings': 426,
          '100m+': 123,
          '150m+': 35,
          '200m+': 9,
          '300m+': 0,
          'Telecom Towers': 1,
          'All Structures': 429
        },
        {
          '#': 26,
          'City': 'Melbourne',
          'Country': 'Australia',
          'All Buildings': 207,
          '100m+': 115,
          '150m+': 40,
          '200m+': 13,
          '300m+': 0,
          'Telecom Towers': 4,
          'All Structures': 211
        },
        {
          '#': 23,
          'City': 'Miami',
          'Country': 'United States',
          'All Buildings': 124,
          '100m+': 98,
          '150m+': 41,
          '200m+': 3,
          '300m+': 0,
          'Telecom Towers': 0,
          'All Structures': 125
        },
        {
          '#': 29,
          'City': 'Houston',
          'Country': 'United States',
          'All Buildings': 195,
          '100m+': 91,
          '150m+': 37,
          '200m+': 15,
          '300m+': 2,
          'Telecom Towers': 1,
          'All Structures': 196
        },
        {
          '#': 12,
          'City': 'Chengdu',
          'Country': 'China',
          'All Buildings': 96,
          '100m+': 90,
          '150m+': 77,
          '200m+': 16,
          '300m+': 0,
          'Telecom Towers': 1,
          'All Structures': 97
        },
        {
          '#': 28,
          'City': 'Istanbul',
          'Country': 'Turkey',
          'All Buildings': 102,
          '100m+': 88,
          '150m+': 38,
          '200m+': 2,
          '300m+': 0,
          'Telecom Towers': 1,
          'All Structures': 103
        },
        {
          '#': 44,
          'City': 'San Francisco',
          'Country': 'United States',
          'All Buildings': 111,
          '100m+': 87,
          '150m+': 21,
          '200m+': 3,
          '300m+': 0,
          'Telecom Towers': 3,
          'All Structures': 114
        },
        {
          '#': 15,
          'City': 'Bangkok',
          'Country': 'Thailand',
          'All Buildings': 115,
          '100m+': 82,
          '150m+': 62,
          '200m+': 12,
          '300m+': 2,
          'Telecom Towers': 1,
          'All Structures': 116
        },
        {
          '#': 14,
          'City': 'Shenyang',
          'Country': 'China',
          'All Buildings': 80,
          '100m+': 79,
          '150m+': 72,
          '200m+': 10,
          '300m+': 2,
          'Telecom Towers': 1,
          'All Structures': 81
        },
        {
          '#': 23,
          'City': 'Mumbai',
          'Country': 'India',
          'All Buildings': 124,
          '100m+': 76,
          '150m+': 41,
          '200m+': 10,
          '300m+': 1,
          'Telecom Towers': 1,
          'All Structures': 125
        },
        {
          '#': 68,
          'City': 'São Paolo',
          'Country': 'Brazil',
          'All Buildings': 176,
          '100m+': 76,
          '150m+': 13,
          '200m+': 0,
          '300m+': 0,
          'Telecom Towers': 0,
          'All Structures': 176
        },
        {
          '#': 17,
          'City': 'Busan',
          'Country': 'South Korea',
          'All Buildings': 84,
          '100m+': 73,
          '150m+': 54,
          '200m+': 15,
          '300m+': 1,
          'Telecom Towers': 0,
          'All Structures': 84
        },
        {
          '#': 19,
          'City': 'Kuala Lumpur',
          'Country': 'Malaysia',
          'All Buildings': 104,
          '100m+': 70,
          '150m+': 53,
          '200m+': 21,
          '300m+': 3,
          'Telecom Towers': 1,
          'All Structures': 107
        },
        {
          '#': 23,
          'City': 'Osaka',
          'Country': 'Japan',
          'All Buildings': 76,
          '100m+': 70,
          '150m+': 41,
          '200m+': 5,
          '300m+': 1,
          'Telecom Towers': 1,
          'All Structures': 78
        },
        {
          '#': 80,
          'City': 'Buenos Aires',
          'Country': 'Argentina',
          'All Buildings': 80,
          '100m+': 69,
          '150m+': 10,
          '200m+': 0,
          '300m+': 0,
          'Telecom Towers': 0,
          'All Structures': 80
        },
        {
          '#': 16,
          'City': 'Nanjing',
          'Country': 'China',
          'All Buildings': 69,
          '100m+': 67,
          '150m+': 55,
          '200m+': 25,
          '300m+': 3,
          'Telecom Towers': 1,
          'All Structures': 70
        },
        {
          '#': 41,
          'City': 'Los Angeles',
          'Country': 'United States',
          'All Buildings': 95,
          '100m+': 67,
          '150m+': 24,
          '200m+': 12,
          '300m+': 2,
          'Telecom Towers': 0,
          'All Structures': 95
        },
        {
          '#': 58,
          'City': 'Atlanta',
          'Country': 'United States',
          'All Buildings': 90,
          '100m+': 67,
          '150m+': 16,
          '200m+': 10,
          '300m+': 1,
          'Telecom Towers': 2,
          'All Structures': 92
        },
        {
          '#': 20,
          'City': 'Panama City',
          'Country': 'Panama',
          'All Buildings': 79,
          '100m+': 66,
          '150m+': 51,
          '200m+': 22,
          '300m+': 0,
          'Telecom Towers': 0,
          'All Structures': 79
        },
        {
          '#': 49,
          'City': 'Mexico City',
          'Country': 'Mexico',
          'All Buildings': 99,
          '100m+': 66,
          '150m+': 19,
          '200m+': 4,
          '300m+': 0,
          'Telecom Towers': 1,
          'All Structures': 100
        },
        {
          '#': 54,
          'City': 'Calgary',
          'Country': 'Canada',
          'All Buildings': 90,
          '100m+': 63,
          '150m+': 17,
          '200m+': 4,
          '300m+': 1,
          'Telecom Towers': 1,
          'All Structures': 91
        },
        {
          '#': 68,
          'City': 'Brisbane',
          'Country': 'Australia',
          'All Buildings': 97,
          '100m+': 60,
          '150m+': 13,
          '200m+': 5,
          '300m+': 0,
          'Telecom Towers': 0,
          'All Structures': 97
        },
        {
          '#': 54,
          'City': 'London',
          'Country': 'United Kingdom',
          'All Buildings': 263,
          '100m+': 59,
          '150m+': 17,
          '200m+': 5,
          '300m+': 1,
          'Telecom Towers': 5,
          'All Structures': 272
        }
      ]
    }
  }
}
</script>
