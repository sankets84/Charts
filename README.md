# Charts
FusionCharts.ready(function () {
    var analysisChart = new FusionCharts({
        type: 'stackedColumn2DLine',
        renderAt: 'chart-container',
        width: '600',
        height: '500',
        dataFormat: 'json',
        dataSource: {
            "chart": {
                "showvalues": "0",
                "caption": "Sales Performance Tracker",
                //"numberprefix": "$",
                "xaxisname": "Months",
                "yaxisname": "Units",
                "showBorder": "0",
                "paletteColors": "#0075c2,#1aaf5d,#f2c500",
                "bgColor": "#ffffff",
                "canvasBgColor": "#ffffff",
                "captionFontSize": "14",
                "subcaptionFontSize": "14",
                "subcaptionFontBold": "0",
                "divlineColor": "#999999",
                "divLineIsDashed": "1",
                "divLineDashLen": "1",
                "divLineGapLen": "1",
                "toolTipColor": "#ffffff",
                "toolTipBorderThickness": "0",
                "toolTipBgColor": "#000000",
                "toolTipBgAlpha": "80",
                "toolTipBorderRadius": "2",
                "toolTipPadding": "5",
                "legendBgColor": "#ffffff",
                "legendBorderAlpha": '0',
                "legendShadow": '0',
                "legendItemFontSize": '10',
                "legendItemFontColor": '#666666'
            },
            "categories": [
                {
                    "category": [
                        {
                            "label": "Nov"
                        },
                        {
                            "label": "Dec"
                        },
                        {
                            "label": "Jan"
                        },
                        {
                            "label": "Feb"
                        }
                    ]
                }
            ],
            "dataset": [
                {
                    "seriesname": "Sales",
                    "data": [
                        {
                            "value": "235000"
                        },
                        {
                            "value": "225100"
                        },
                        {
                            "value": "222000"
                        },
                        {
                            "value": "230500"
                        }
                    ]
                },
                {
                    "seriesname": "Orders",
                    "data": [
                        {
                            "value": "230000"
                        },
                        {
                            "value": "143000"
                        },
                        {
                            "value": "198000"
                        },
                        {
                            "value": "327600"
                        }
                    ]
                },
                {
                    "seriesname": "YTD",
                    "data": [
                        {
                            "value": "130000"
                        },
                        {
                            "value": "103000"
                        },
                        {
                            "value": "108000"
                        },
                        {
                            "value": "127600"
                        }
                    ]
                },
                {
                    "seriesname": "Average",
                    "renderas": "Line",
                    "data": [
                        {
                            "value": "455000"
                        },
                        {
                            "value": "334000"
                        },
                        {
                            "value": "426000"
                        },
                        {
                            "value": "403000"
                        }
                    ]
                },
                {
                    "seriesname": "Three Year Average",
                    "renderas": "Line",
                    "data": [
                        {
                            "value": "495000"
                        },
                        {
                            "value": "374000"
                        },
                        {
                            "value": "466000"
                        },
                        {
                            "value": "443000"
                        }
                    ]
                }
            ]
        }
    }).render();
});
