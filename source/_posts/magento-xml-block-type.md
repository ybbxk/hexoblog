title: Magento的block type解释
date: 2016-02-23 22:46:38
tags:
---
Magento在xml文件中block的type解释。结果也是在网上搜到的，按照 `type="A/B"`的格式来解释。
The A is a module's alias. In this case page is short for Mage_Page_Block (it is defined in app/code/core/Mage/Page/etc/config.xml if you want to see).
The B is the class name relative to the alias, initial letters of each word are capitalised. In this case html becomes Html and is appended to the resolved alias, so it is Mage_Page_Block_Html. This is probably found in the file app/code/core/Mage/Page/Block/Html.php because class names translate directly to locations in Magento.
Were you using a model alias instead of a block alias then page would be Mage_Page_Model instead. The same thing happens for resource models and helpers too. Your own module will need to define these in it's config if it is to have blocks, models and helpers.
[链接](http://stackoverflow.com/questions/6633307/understanding-magento-block-and-block-type)

