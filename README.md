# react-datetime-picker

> Made with create-react-library

[![NPM](https://img.shields.io/npm/v/react-datetime-picker.svg)](https://www.npmjs.com/package/react-datetime-picker) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save react-datetime-picker
```

## Usage

```tsx
import React, { Component } from 'react'

import { DtPicker } from 'react-datetime-picker'
import 'react-datetime-picker/dist/index.css'

const App = () => {
  const [date, setDate] = useState()
  const handleCalendarClose = () => console.log('Calendar closed')
  const handleCalendarOpen = () => console.log('Calendar opened')
  return (
      <DtPicker
        onChange={setDate}
        defaultValue={date}
        type='single'
        local='en'
        withTim
        showWeekend
        clearBtn
        onCalenderShow={handleCalendarOpen}
        onCalenderHide={handleCalendarClose}
        // isDisabled
      />
  )
}
```
### TODO

- [ ] max date
- [ ] min date
- [ ] check init value and min max (max must be greater than min)
- [ ] fix header change view form months to years
- [ ] Portal version ( search portal in https://reactdatepicker.com/)
- [ ] add today button
- [ ] add auto close form calender without time
- [ ] remove disabled date in range date
- [ ] write test
- [ ] add styles

## License

MIT © [mehdinasiri](https://github.com/mehdinasiri)
