# Chart
Test for code block

## JSON
```
{% chart %}
{
    "data": {
        "type": "bar",
        "columns": [
            ["data1", 30, 200, 100, 400, 150, 250],
            ["data2", 50, 20, 10, 40, 15, 25]
        ],
        "axes": {
            "data2": "y2"
        }
    },
    "axis": {
        "y2": {
            "show": true
        }
    }
}
{% endchart %}
```

{% chart %}
{
    "data": {
        "type": "bar",
        "columns": [
            ["data1", 30, 200, 100, 400, 150, 250],
            ["data2", 50, 20, 10, 40, 15, 25]
        ],
        "axes": {
            "data2": "y2"
        }
    },
    "axis": {
        "y2": {
            "show": true
        }
    }
}
{% endchart %}

### YAML
```
{% chart format="yaml" %}
data:
    columns:
        - [data1, 30, 200, 100, 400, 150, 250]
        - [data2, 50, 20, 10, 40, 15, 25]
    axes:
        data2: y2
axis:
    y2:
        show: true
{% endchart %}
```

{% chart format="yaml" %}
data:
    columns:
        - [data1, 30, 200, 100, 400, 150, 250]
        - [data2, 50, 20, 10, 40, 15, 25]
    axes:
        data2: y2
axis:
    y2:
        show: true
{% endchart %}
