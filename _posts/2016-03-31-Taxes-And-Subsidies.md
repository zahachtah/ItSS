---
title: "Taxes and subsidies"
categories:
  - Governance
tags:
  - image
  - Post Formats
author_profile: false
sidebar:
  nav: sideMenu
---

# Introduction to taxes

**Taxes** are the main source of financing for government activities, such as administration of governance and public goods and services. Taxes also can be used to change consumer behavior and/or to attempt to correct certain market failures.

What about a road or a beach? If few people use them, these resources appear to be public goods because they are not consumed (subtracted as for fishery) and hence there seem to be as much left for others to enjoy. However, this is not correct and this will become more evident the more people who use them. These resources are called ‘congestion goods’ because at least in theory there will be a user intensity that creates cost, congestion, for other users (imaging a crowded beach or traffic queues). To avoid congestion economists recommend user charges like entrance fees to beaches and congestion tax for driving in cities.

The graph below illustrates some basic fundamentals related to taxes in our demand/supply context. In this case we are looking at a tax on production i.e. a tax paid by the firms. The tax implies that producers will have to charge more for each quantity of the product they produce. This causes an upward shift in their marginal cost curves and hence an upward shift in the aggregate supply curve by an amount equal to the size of the tax.Consumers are thus paying p~consumer~ and hence adjust their demand to this price. As can be seen in the graph this causes a new market equilibrium to form at q~tax~. Producers thus charge a higher price p~consumer~ but are also forced to pay tax to the government. The size of the tax payment is illustrated by the orange area which is the tax income collected by the government.

# Taxes Figure:

<div id="boxTax"></div>


As can be seen, both consumer surplus (green area) and producer surplus (violet area) is reduced as you increase the taxation. Which will be reduced the most will depend on the slopes of the demand and supply curves. The slopes are usually referred to as the elasticity of demand and supply. However, the tax collected by the government can now be used by the government to finance education, health, nature conservation, child benefits, elderly or those unemployed, or other things that enhance human wellbeing and equity. This illustrates the basic purpose of a tax, which is an important means of income redistribution in society today.




# Introduction to subsidies

Education is mainly a private benefit but the whole society benefits also from a higher level of education (i.e. external benefit) and this justifies that almost all countries in the world subsidise primary education. What about biodiversity and ecosystem services (ES)? To a large extent it is beneficial for farmers if there are pollinating insects and if aphids and weeds are controlled by “natural enemies,” such as birds and insects, so that the farmer need not to use pesticides. If it was only a private benefit there would be no reason for society to subsidise it.

However, biodiversity and ES are also public goods since a large part of the benefits cannot be reaped by the farmers. Biodiversity and ES are both an input to agriculture, because they increase harvest and the resilience to various disturbances; and an output from agriculture, because farming can have positive or negative effects on biodiversity, water quality, soil carbon, frequency of pollinating insects, etc. And these outputs are to a large extent external costs and external benefits. But a farmer should not have to pay for the production of public goods if it reduces his income from using his land for production.

This justifies policies, both carrots and sticks. Carrots are both taxes and subsidies that leave the decision to farmers but try to influence behaviour. Sticks are quantitative regulations and prohibitions from using dangerous pesticides, especially near water.  In Europe, the Common Agricultural Policy (CAP) supports organic farming, grasslands and other land-use that is believed to enhance biodiversity and several ES.

In the figure below we assume that the demand (willingness-to-pay) for grasslands is substantially higher for the public than for the individual farmer; it is mainly an external benefit of keeping open landscape with high biodiversity values. It is also a public good because the benefit is enjoyed in a way that does not reduce the benefits for others. We assume that the benefit from grasslands decreases with the area of grasslands since not all grassland is needed to produce the benefits. In reality this curve is probably non-linear but we keep it linear for simplicity. The cost in this case is the opportunity cost, i.e. forgone net benefits of using the land for the best alternative management such as crop production. If the best alternative is to produce wheat, then the cost of producing a grassland is the cost of the grassland plus the forgone net benefit of wheat. A stony permanent natural pasture is of little value (to the farmer) for wheat but the farmer may plant spruce or other trees if society does not pay her to produce grassland.

The demand of the farmer and the demand of society should be added vertically, instead of horizontally as e.g. for wheat and beef. The optimal supply of grasslands corresponds to a 100% payment. This will generate a consumer surplus for society and a producer surplus for the farmer(s) because some grasslands can be provided at a low cost.

The implicit assumption in this reasoning is that farmers have property rights to decide on land-use. The state therefore has to ‘bribe’ the farmer to choose an alternative land-use, which sometimes is called the ‘producer-receives-principle’ (PRP). A reverse situation would be that the government only allowed land-use with little negative externalities and that the farmer would need to pay a fee (economists often use the word ‘bribe’) to plant wheat instead (assuming wheat was associated with nitrogen leakage). This could be justified by the more common polluter-pays-principle (PPP). However, according to the Swedish Constitution 2:15, farmers have the right to continue on-going land-use and if the government wants to interfere they need to pay full compensation and can only do so if it is in the public’s best interest.

In the figure below, increase the subsidy to change the incentive of the farmer to change the land use from crop production to grasslands.


# Subsidies Figure:

<div id="boxSub"></div>


## Contributors

Thomas Hahn, Jon Norberg

<style>
#boxTax {
    width:700px;
    height:500px;
    margin: 0 4em 1em 0;
    float: left;
}
#boxSub {
    width:700px;
    height:500px;
    margin: 0 4em 1em 0;
    float: left;
}
  .JXGtext {
    background-color:transparent;
    font-family: Arial, Helvetica, Geneva;
    font-size:11px;
    padding:0px;
    margin:0px;
  }
</style>

<script src="https://jsxgraph.uni-bayreuth.de/distrib/jsxgraphcore.js"></script>
<script>
JXG.Options.axis.ticks.majorHeight = 40; // removes larger grid
JXG.Options.axis.ticks.drawLabels = false;
JXG.Options.axis.ticks.insertTicks = false;
JXG.Options.axis.lastArrow = false;
var b = JXG.JSXGraph.initBoard('boxTax', {boundingbox: [-0.2, 1.1, 1.1, -0.2], axis: true,showNavigation:false,showCopyright:false});

    u = b.createElement('slider', [
        [0.0, -0.05],
        [1.0, -0.05],
        [0, 0, 1]
    ], {
        name: '&epsilon;',
        strokeColor: 'black',
        fillColor: 'black'
    });
    ut = b.createElement('text', [0.5, -0.1, "Tax"], {
        fixed: true
    });




//The value of s is"+s.Value().toFixed(2)

//var checkbox = b.create('checkbox', [0.25, 0.5, 'Change Y'], {});

    var chk = b.create('text', [0.01,-0.1,
            '<input type="checkbox" id="showU" onchange="toggleUpper()" unchecked/>  Welfare benefit<br/>'
                               ],{strokeColor:'#1f78b4'});

    var upperVisible = true;
    var toggleUpper = function() {
            upperVisible = !upperVisible;
        if (upperVisible==true) {
            h.setProperty({fillOpacity:0.5});
            h.setProperty({strokeColor:false});
        }
        else
        {
            h.setProperty({fillOpacity:1});
            h.setProperty({strokeColor:true});
        }
        };

var q=2
var col1='silver'
var col2='grey'
var polygonColor='#1f78b4'
var helperColor=false//'#888888'//false
var helperLabel=false
var slideFactor=1.5
var taxRevCol='#ff7f00'
var prodSurCol='#6a3d9a'
var conSurCol='#b2df8a'
var welfOpac=0.5




var p1 = b.create('point',[0,1],{size:1,strokeColor:col1,fillColor:col1,withLabel:false});
var p2 = b.create('point',[1,0],{size:1,strokeColor:col1,fillColor:col1,withLabel:false});
var p3 = b.create('point',[1,1],{size:1,strokeColor:col1,fillColor:col1,withLabel:false});
var p4 = b.create('point',[0,0.3],{size:1,strokeColor:col1,fillColor:col1,withLabel:false});
var q1 = b.create('point',[0.6,0.3],{size:5,fillColor:'red', name:'Demand', labelColor:col2,face:'+',label:{strokeColor:'red'}});
var q2 = b.create('point',[0.6,0.6],{size:5,fillColor:'blue',strokeColor:'blue', name:'Supply',face:'+',label:{strokeColor:'blue'}});

var p4TS = b.create('point',[function(){ return (p4.X());},function(){ return (p4.Y()*(1+slideFactor*u.Value()));}],{size:0,strokeColor:col1,fillColor:col1,withLabel:false});
var p3TS = b.create('point',[function(){ return (p3.X());},function(){ return (p3.Y()*(1+slideFactor*u.Value()));}],{size:0,strokeColor:col1,fillColor:col1,withLabel:false});
var q2TS = b.create('point',[function(){ return (q2.X());},function(){ return (q2.Y()*(1+slideFactor*u.Value()));}],{size:0,strokeColor:col1,fillColor:col1,withLabel:false});


var Demand = b.create('curve', JXG.Math.Numerics.bezier([p1,q1,q1,p2]),{strokecolor:'red', strokeWidth:3});
var Supply = b.create('curve', JXG.Math.Numerics.bezier([p3,q2,q2,p4]),{strokecolor:'blue', strokeWidth:3});
var SupplyTS = b.create('curve', JXG.Math.Numerics.bezier([p3TS,q2TS,q2TS,p4TS]),{strokecolor:'blue', strokeWidth:2, dash:2});


var SD = b.create('intersection', [Supply, Demand, 0],{size:3,strokeColor:false,fillColor:helperColor,withLabel:helperLabel,name:'SD'});
var SD0 = b.create('point',[function(){ return (SD.X());},0],{name:'Q_{no tax}',size:3,withLabel:false});
var SDY = b.create('point',[0,function(){ return (SD.Y());}],{size:3,strokeColor:false,fillColor:helperColor,withLabel:helperLabel,name:'SDY'});
var SD0S=b.create('segment',[SD,SDY],{strokeColor:helperColor,dash:2})

var SDTS = b.create('intersection', [SupplyTS, Demand, 0],{size:3,strokeColor:false,fillColor:helperColor,withLabel:helperLabel,name:'SDTS'});
var SDTS0=b.create('point',[function(){ return (SDTS.X());},0],{size:3,strokeColor:false,fillColor:helperColor,withLabel:true,name:'q_{produced}'});
var QstarLine=b.create('segment',[SDTS,SDTS0],{strokeColor:helperColor,dash:2})
var pProd=b.create('intersection',[QstarLine,Supply],{size:3,strokeColor:false,fillColor:helperColor,withLabel:helperLabel,name:'pProd'});
var pProd0=b.create('point',[0,function(){ return (pProd.Y());}],{size:3,strokeColor:false,fillColor:helperColor,withLabel:helperLabel,name:'pProd0'});
var pProdS=b.create('segment',[pProd,pProd0],{strokeColor:helperColor,dash:2})

var XYZ=b.create('intersection',[SD0S,QstarLine],{size:3,strokeColor:false,fillColor:helperColor,withLabel:helperLabel,name:'XYZ'});

var Pstar=b.create('point',[0,function(){ return (SDTS.Y());}],{size:3,strokeColor:false,fillColor:helperColor,withLabel:true,name:'P_{consumer}'});
var PstarLine=b.create('segment',[Pstar,SDTS],{strokeColor:helperColor,dash:2})

var helpLine=b.create('line',[SD,SD0],{strokeColor:helperColor,dash:2})
var SDTSh = b.create('intersection', [SupplyTS, helpLine, 0],{size:3,strokeColor:false,fillColor:helperColor,withLabel:helperLabel,name:'SDTSh'});
var Int2 = b.create('intersection', [SupplyTS, SD0S, 0],{size:3,strokeColor:false,fillColor:helperColor,withLabel:helperLabel,name:'Int2'});


var h = b.create('polygon', [SD, SDTS, SDTSh,SD],{name:'h',size:3,fillcolor:polygonColor, strokeColor:false,withLabel:helperLabel, fillOpacity:0.5});
var d = b.create('polygon', [SD, XYZ, SDTS,SD],{name:'d',size:3,fillcolor:polygonColor, strokeColor:false,withLabel:helperLabel, fillOpacity:0.5});
var e = b.create('polygon', [SD, XYZ, pProd],{name:'e',size:3,fillcolor:polygonColor, strokeColor:false,withLabel:helperLabel, fillOpacity:0.5});
var conSur = b.create('polygon', [SDTS, Pstar, p1],{name:'conSur',size:3,fillcolor:conSurCol, strokeColor:false,withLabel:helperLabel, fillOpacity:0.5});

var taxRev = b.create('polygon', [pProd, SDTS, Pstar,pProd0],{name:'TaxRev',size:3,fillcolor:taxRevCol, strokeColor:false,withLabel:helperLabel, fillOpacity:0.5});

var prodSur = b.create('polygon', [pProd, p4, pProd0],{name:'prodSur',size:3,fillcolor:prodSurCol, strokeColor:false,withLabel:helperLabel, fillOpacity:0.5});

    taxT = b.createElement('text', [0.05, -0.15, function(){return (h.Area()*100).toFixed(2);}], {
        fixed: true
    });
</script>

<script>
//remeber to set on load in jsfiddle


JXG.Options.axis.ticks.majorHeight = 40; // removes larger grid
JXG.Options.axis.ticks.drawLabels = false;
JXG.Options.axis.ticks.insertTicks = false;
JXG.Options.axis.lastArrow = false;
var b = JXG.JSXGraph.initBoard('boxSub', {boundingbox: [-0.05, 1.1, 1.1, -0.2], axis: true,showNavigation:false,showCopyright:false});



var q=2
var col1='silver'
var col2='grey'
var polygonColor='#1f78b4'
var helperColor=false//'#888888'//false
var helperLabel=false
var slideFactor=10
var taxRevCol='#ff7f00'
var prodSurCol='#6a3d9a'
var conSurCol='#b2df8a'
var welfOpac=0.5

    u = b.createElement('slider', [
        [0.0, -0.12],
        [1.0, -0.12],
        [0, 0, 1]
    ], {

        strokeColor: 'black',
        fillColor: 'black'
    });

    ut = b.createElement('text', [0.45, -0.18, "Subsidy"], {fixed: true, strokecolor:'green'});

    PublicD = b.createElement('text', [0.1, 0.94, "Public demand"], {fixed: true, strokecolor:'red'});



farmerMC = b.createElement('text', [0.83, 0.8, "Farmer Cost"], {fixed: true, strokecolor:'blue'});

    Xlabel = b.createElement('text', [0.9, -0.05, "Grasslands (ha)"], {fixed: true});

var p1 = b.create('point',[0,1],{size:1,strokeColor:col1,fillColor:col1,withLabel:helperLabel});
var p2 = b.create('point',[1,0],{size:1,strokeColor:col1,fillColor:col1,withLabel:helperLabel});
var p3 = b.create('point',[1,1],{size:1,strokeColor:col1,fillColor:col1,withLabel:helperLabel});
var p4 = b.create('point',[0,0.05],{size:1,strokeColor:col1,fillColor:col1,withLabel:helperLabel});
var p5 = b.create('point',[0,0.1],{size:1,strokeColor:col1,fillColor:col1,withLabel:helperLabel});
var p6 = b.create('point',[1,0.0],{size:1,strokeColor:col1,fillColor:col1,withLabel:helperLabel});
var p7 = b.create('point',[function(){ return (p5.X());},function(){ return (p5.Y()*(1+slideFactor*u.Value()));}],{size:0,strokeColor:col1,fillColor:col1,withLabel:false});


var SDemand = b.create('segment', [p1,p2],{strokecolor:'red', strokeWidth:1});
var Supply = b.create('segment', [p3,p4],{strokecolor:'blue', strokeWidth:2});
var FDemand = b.create('segment', [p5,p6],{strokecolor:'red', strokeWidth:1});
var FTDemand = b.create('segment', [p7,p6],{strokecolor:'green', strokeWidth:1, dash: 2});


var IF = b.create('intersection', [Supply, FDemand, 0],{size:3,strokeColor:false,fillColor:helperColor,withLabel:helperLabel});
var IS = b.create('intersection', [Supply, SDemand, 0],{size:3,strokeColor:false,fillColor:helperColor,withLabel:helperLabel});
var I1 = b.create('intersection', [Supply, FTDemand, 0],{size:3,strokeColor:false,fillColor:'green',withLabel:helperLabel});


var LineIF = b.create('segment', [IF,[function (){return IF.X()},0]],{strokecolor:'grey', strokeWidth:2, dash: 2});

var LineIS = b.create('segment', [IS,[function (){return IS.X()},0]],{strokecolor:'grey', strokeWidth:2, dash: 2});

var LineI1 = b.create('segment', [I1,[function (){return I1.X()},0]],{strokecolor:'green', strokeWidth:2});

var FarmerGrass = b.create('point',[function (){return I1.X()},0],{size:1,strokeColor:col1,fillColor:col1,withLabel:true,name:"F_{grassland}(ha)"});

    farmerD = b.createElement('text', [function (){return 0.03+I1.X()}, function (){return 0.01+I1.Y()}, "Farmer demand"], {fixed: true, strokecolor:'green'});


</script>
