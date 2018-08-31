```javascript
$(function () {
    const test = $('#box').numberRun({
        speed: '2s',
        num: 1224.15,
        style: {
            'height': '30px',
            'width': '20px',
            'font-size': '30px'
        }
    });
    const test2 = $('#box2').numberRun({
        speed: '0.3s',
        num: 12223.13,
        style: {
            'height': '16px',
            'width': '12px',
            'font-size': '14px'
        }
    });
    const test3 = $('#box3').numberRun({
        speed: '0.3s',
        num: 342.551,
        style: {
            'height': '16px',
            'width': '14px',
            'font-size': '16px',
            'background-color': '#000',
            'color': '#fff',
            'margin-right': '5px'
        }
    });
    setInterval(() => {
        let num = math.eval($('#box').find('.number-run').attr('data-num') + ' + 3000.23');
        test.run(num.toFixed(2));
        let num2 = math.eval($('#box2').find('.number-run').attr('data-num') + ' + 200.21')
        test2.run(num2.toFixed(2));
        let num3 = math.eval($('#box3').find('.number-run').attr('data-num') + ' + 3421.238')
        test3.run(num3.toFixed(3));
    }, 2000)
})
```
