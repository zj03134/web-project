<template>
  <basic-container>
    <h3>表格例子</h3>
	<avue-input></avue-input>
    <avue-crud :option="option"
               :page="page"
               :data="data"></avue-crud>
  </basic-container>
</template>

<script>
export default {
  data() {
    return {
      page: {
        total: 122
      },
      data: [
        {
          username: "新华微评·学习笔谈：中国的发展是世界的机遇",
          name: "国内新闻",

          date: "2019-01-01",
          textarea: "在巴西利亚举行的金砖国家工商论坛闭幕式上，习近平主席纵论全球经济形势，再次向各国发出合作共赢的诚挚邀请：“中国的发展是世界的机遇。”"
        },
        {
          username: "新华微评·学习笔谈：中国的发展是世界的机遇",
          name: "国内新闻",
          date: "2019-01-01",
          textarea: "习近平在金砖国家领导人巴西利亚会晤公开会议上的讲话（全文）"
        },

        {
          username: "新华微评·学习笔谈：中国的发展是世界的机遇",
          name: "国内新闻",
          date: "2019-01-01",
          textarea: "习近平在金砖国家领导人巴西利亚会晤公开会议上的讲话（全文）"
        },
        {
          username: "新华微评·学习笔谈：中国的发展是世界的机遇",
          name: "国内新闻",
          date: "2019-01-01",
          textarea: "习近平在金砖国家领导人巴西利亚会晤公开会议上的讲话（全文）"
        },
        {
          username: "新华微评·学习笔谈：中国的发展是世界的机遇",
          name: "国内新闻",
          date: "2019-01-01",
          textarea: "习近平在金砖国家领导人巴西利亚会晤公开会议上的讲话（全文）"
        },
        {
          username: "新华微评·学习笔谈：中国的发展是世界的机遇",
          name: "国内新闻",
          date: "2019-01-01",
          textarea: "习近平在金砖国家领导人巴西利亚会晤公开会议上的讲话（全文）"
        },
        {
          username: "新华微评·学习笔谈：中国的发展是世界的机遇",
          name: "国内新闻",
          date: "2019-01-01",
          textarea: "习近平在金砖国家领导人巴西利亚会晤公开会议上的讲话（全文）"
        }
      ],
      option: {
        column: [
          {
            label: "新闻标题",
            prop: "username",
            span: 14,
            row: true
          },
          {
            label: "栏目分类",
            prop: "name",
            span: 14,
            row: true
          },
          {
            label: "新闻时间",
            prop: "date",
            type: "date",
            span: 14,
            row: true
          },
          {
            label: "新闻内容",
            prop: "textarea",
            type: "textarea",
            minRows: 8,
            span: 24,
            overHidden: true,
            row: true,
			
          }
        ]
      }
    };
  }
};
</script>

<style>

</style>
