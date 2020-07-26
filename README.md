# react-native-star-widget

![Screenshot](https://github.com/benediktviebahn/react-native-star-rating-widget/raw/master/media/screenshot.png)

## Installation
1. install react-native-star-widget
`npm install react-native-star-rating-widget --save` or `yarn add react-native-star-rating-widget`
2. if not already installed, add [react-native-svg](https://github.com/react-native-community/react-native-svg)

## Usage
```js
import StarRating from 'react-native-star-rating-widget';

const Example = () => {
  const [rating, setRating] = useState(0);
  return (
      <StarRating
        rating={rating}
        onChange={setRating}
      />
  );
};
```

## Props
| Name       | Type                 | Default         | Description                                      |
| ---------- | -------------------- | --------------- | ------------------------------------------------ |
| rating     | number               | **REQUIRED**    | Rating Value. Should be between 0 and `maxStars` |
| onChange   | (number) => void     | **REQUIRED**    | called when rating changes                       |
| maxStars   | number               | 5               | number of stars                                  |
| minRating  | number               | 0.5             | minimum selectable rating                        |
| starSize   | number               | 32              | star size                                        |
| color      | string               | "#fdd835"       | star color                                       |
| emptyColor | string               | same as `color` | empty star color                                 |
| style      | object               | undefined       | optional style                                   |