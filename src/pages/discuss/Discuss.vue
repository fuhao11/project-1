<template>
    <div class="discuss">
        <discuss-header></discuss-header>
        <discuss-zone :list="list"></discuss-zone>
    </div>
</template>

<script>
import DiscussHeader from './children/Header'
import DiscussZone from './children/Zone'
export default {
    name: "Discuss",
    data () {
        return {
            list:[{
                'head': 'https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=320178652,790985626&fm=26&gp=0.jpg',
                'name': '张三',
                'userid': 'zhangsan',
                'star': 4,
                'content':[{
                    'text': '',
                    'photo': ['https://img.alicdn.com/bao/uploaded/i1/O1CN01VdpIeB1wFpSPthRbm_!!0-rate.jpg_400x400.jpg','https://img.alicdn.com/bao/uploaded/i1/O1CN01VdpIeB1wFpSPthRbm_!!0-rate.jpg_400x400.jpg','https://img.alicdn.com/bao/uploaded/i1/O1CN01VdpIeB1wFpSPthRbm_!!0-rate.jpg_400x400.jpg']
                }],
                'time': '2019.09.24'
            },{
                'head': 'https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=320178652,790985626&fm=26&gp=0.jpg',
                'name': '李四',
                'userid': 'lisi',
                'star': 2,
                'content':[{
                    'text': '',
                    'photo': []
                }],
                'time': '2019.09.24'
            },{
                'head': 'https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=320178652,790985626&fm=26&gp=0.jpg',
                'name': 'wangwu',
                'userid': 'wangwu',
                'star': 3,
                'content':[{
                    'text': '',
                    'photo': ['https://img.alicdn.com/bao/uploaded/i1/O1CN01VdpIeB1wFpSPthRbm_!!0-rate.jpg_400x400.jpg','https://img.alicdn.com/bao/uploaded/i1/O1CN01VdpIeB1wFpSPthRbm_!!0-rate.jpg_400x400.jpg']
                }],
                'time': '2019.09.24'
            },{
                'head': 'https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=320178652,790985626&fm=26&gp=0.jpg',
                'name': '马六',
                'userid': 'maliu',
                'star': 1,
                'content':[{
                    'text': '',
                    'photo': []
                }],
                'time': '2019.09.24'
            }]
        }
    },
    components: {
        DiscussHeader,
        DiscussZone
    }
}
</script>

<style lang="stylus">
    .discuss
        width:100%
        height:100%
        padding-bottom:2rem
        background:#eee
</style>