<template>
    <v-table :width="500" :height="300" 
    tableType="new" :columns="columns" 
    :table-data="tableData" 
    :show-vertical-border="false"
     :select-all="selectALL"
                :select-change="selectgetwatChange"
                @on-custom-comp="customCompFunc"></v-table>
</template>


<script>

    export default{
        data() {
            return {
                 tableData: [
                     {"name":"赵伟","tel":"156*****1987","hobby":"钢琴、书法、唱歌","address":"上海市黄浦区金陵东路569号17楼"},
                     {"name":"李伟","tel":"182*****1538","hobby":"钢琴、书法、唱歌","address":"上海市奉贤区南桥镇立新路12号2楼"},
                     {"name":"孙伟","tel":"161*****0097","hobby":"钢琴、书法、唱歌","address":"上海市崇明县城桥镇八一路739号"},
                     {"name":"周伟","tel":"197*****1123","hobby":"钢琴、书法、唱歌","address":"上海市青浦区青浦镇章浜路24号"},

                     {"name":"赵伟1","tel":"156*****1987","hobby":"钢琴、书法、唱歌","address":"上海市黄浦区金陵东路569号17楼"},
                     {"name":"李伟1","tel":"182*****1538","hobby":"钢琴、书法、唱歌","address":"上海市奉贤区南桥镇立新路12号2楼"},
                     {"name":"孙伟2","tel":"161*****0097","hobby":"钢琴、书法、唱歌","address":"上海市崇明县城桥镇八一路739号"},
                     {"name":"周伟2","tel":"197*****1123","hobby":"钢琴、书法、唱歌","address":"上海市青浦区青浦镇章浜路24号"},
                     {"name":"赵伟","tel":"156*****1987","hobby":"钢琴、书法、唱歌","address":"上海市黄浦区金陵东路569号17楼"},
                     {"name":"李伟","tel":"182*****1538","hobby":"钢琴、书法、唱歌","address":"上海市奉贤区南桥镇立新路12号2楼"},
                     {"name":"孙伟","tel":"161*****0097","hobby":"钢琴、书法、唱歌","address":"上海市崇明县城桥镇八一路739号"},
                     {"name":"周伟","tel":"197*****1123","hobby":"钢琴、书法、唱歌","address":"上海市青浦区青浦镇章浜路24号"},

                     {"name":"赵伟1","tel":"156*****1987","hobby":"钢琴、书法、唱歌","address":"上海市黄浦区金陵东路569号17楼"},
                     {"name":"李伟1","tel":"182*****1538","hobby":"钢琴、书法、唱歌","address":"上海市奉贤区南桥镇立新路12号2楼"},
                     {"name":"孙伟2","tel":"161*****0097","hobby":"钢琴、书法、唱歌","address":"上海市崇明县城桥镇八一路739号"},
                     {"name":"周伟2","tel":"197*****1123","hobby":"钢琴、书法、唱歌","address":"上海市青浦区青浦镇章浜路24号"},
                 ],
                columns: [
                     {width: 60, titleAlign: 'center',columnAlign:'center',type: 'selection'},
                    {field: 'name', title:'姓名', width: 100, titleAlign: 'center',columnAlign:'center'},
                    {field: 'tel', title: '手机号码', width: 260, titleAlign: 'center',columnAlign:'center'},
                    // {field: 'hobby', title: '爱好', width: 330, titleAlign: 'center',columnAlign:'center'},
                    // {field: 'address', title: '地址', titleAlign: 'center',columnAlign:'left'}
                ]
            }
        },

        methods:{
            selectgetwatChange(selection, rowData) {
                console.log('selection,',selection,'rowData=',rowData)
            }
        }
    }
</script>
<style scoped>
.v-table-body-class{
    border:1px solid rgb(245, 231, 231);
}
.v-table-class{

    border:0px solid rgb(245, 231, 231);
}
</style>