# Tatiana Shestakova
### *Frontend Developer*
***
## Details
- **Born**: Beloretsk, Russia. November 9, 1993 
- **Location**: Bourne, UK
- **Email**: tatjana.shestackowa93@gmail.com
- **GitHub**: [@tshshshsh](https://github.com/tshshshsh)

***
## Skills
- HTML5, CSS3, JavaScript (ES6+)
- React, Next.js, Tailwind CSS
- Git, GitHub
- Figma

***
## Languages
- Russian - Native
- English - B2-C1

***
## Courses
![rs-stage0](/assets/rs-stage-0.png)

***
## Code example
```
function formatDuration (seconds) {
  const sec = seconds % 60;
  
  const allMin = Math.floor(seconds / 60);
  const min = allMin % 60;
  
  const allHours = Math.floor(allMin / 60);
  const hours = allHours % 24;
  
  const allDays = Math.floor(allHours / 24);
  const days = allDays % 365;
  
  const years = Math.floor(allDays / 365);
   
  const timeResult = [
    {type: 'years', value: years},
    {type: 'days', value: days},
    {type: 'hours', value: hours},
    {type: 'min', value: min},
    {type: 'sec', value: sec}
  ];
  
  const dictionary = {
    years: {sin: 'year', pl: 'years'},
    days: {sin: 'day', pl: 'days'},
    hours: {sin: 'hour', pl: 'hours'},
    min: {sin: 'minute', pl: 'minutes'},
    sec: {sin: 'second', pl: 'seconds'}
  };
  
  const values = timeResult.filter(({value}) => value > 0)
    .map(({type, value}) => value > 1 ? (value + ' ' + dictionary[type]['pl']):
         (value + ' ' + dictionary[type]['sin'])
        );
  
  if (values.length === 0) {
    return 'now';
  }
  if (values.length === 1) {
    return values[0];
  }
  if (values.length === 2) {
    return values[0] + ' and ' + values[1];
  }
  return values.slice(0,-1).join(', ') + ' and ' + values[values.length - 1]
}
```

