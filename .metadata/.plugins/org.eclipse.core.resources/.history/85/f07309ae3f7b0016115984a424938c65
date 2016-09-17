package com.taotao.manage.service;

import java.util.List;

import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Service;

import com.taotao.manage.mapper.ItemCatMapper;
import com.taotao.manage.pojo.ItemCat;

@Service
public class ItemCatService {

    @Autowired
    private ItemCatMapper itemCatMapper;
    
    //
    public List<ItemCat> queryItemCat(Long parentId){
        ItemCat itemCat = new ItemCat();
        itemCat.setParentId(parentId);
        return this.itemCatMapper.select(itemCat);
    }
}
