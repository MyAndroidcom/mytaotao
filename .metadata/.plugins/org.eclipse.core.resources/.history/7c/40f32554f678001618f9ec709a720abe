package com.taotao.manage.service;

import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Service;

import com.taotao.manage.pojo.Item;
import com.taotao.manage.pojo.ItemDesc;

@Service
public class ItemService extends BaseService2<Item> {
    @Autowired
    private ItemDescService itemDescService;
    
    public void saveItem(Item item,String desc){
        //设置初始数据
        item.setStatus(1);
        item.setId(null);
        super.save(item);
        
        ItemDesc itemDesc = new ItemDesc();
        itemDesc.setItemId(item.getId());
        itemDesc.setItemDesc(desc);
        this.itemDescService.save(itemDesc);
    }
}
