# How To Create and Review Documents

[How to create a new document]()

[How to review a document]()

## How to CREATE a new document?

{% hint style="warning" %}
Always create files on Gitbook first. Files created outside Gitbook are sometimes not correctly tracked and you might risk not seeing your changes in Gitbook later.
{% endhint %}

If you want to create a new document, follow these steps:

1. First, you need to create a new branch that will hold your draft until it is ready for review.
   1. In the left sidebar, click on `New` -&gt; `New variant`. This will create a new branch which will automatically be in sync with Github.
   2. Under "Variant Name", type the name of your new branch, which must be of the form `draft/<document-topic>`.
   3. Click `Create`. Note that, in the top left, Gitbook shows that you are now editing in your branch. All of the changes you make will be contained within this branch until you create a pull request and merge your edits back into `master`.
2. Next, you need to create a new document.
   1. Click on `New` -&gt; `New page`. This will create a blank document.
   2. Drag the new document to the appropriate section in the left sidebar. For example, if you are creating a new ADR, drag the document to the end of the "Architectural Decision Records" section.
   3. Give your document a title. _If you're creating an ADR, your title must start with the four-digit, zero-padded index one higher than the last document in the ADR section._
3. Finally, in the bottom left, click `Save`, then `Merge`. This will merge your changes into your new branch \(note that this is not a merge to `master`\).
4. You can now edit your document. If creating an ADR or SDS, begin by copying and pasting from the [ADR Template]() or [SDS Template](). \(Currently you cannot directly clone templates in Gitbook, but you should be able to [soon](https://gitbook.canny.io/feature-requests/p/action-to-duplicate-pages).\)
   * **On  Gitbook**: Use the inline editor to modify the document. Afterwards `Save` and `Merge` your edits. You can always come back and continue working on your draft. While working on your draft in Gitbook, others will be able to check out the branch/variant and leave comments, which you can resolve afterwards.
   * **On Github** You can also edit the files directly on [Github](https://github.com/wri/.core-api), or clone the repository and use the desktop editor of your choice.  Once done, commit your changes. If working offline, make sure you push your changes back to the `draft/` branch you are working in. Changes you make directly to your branch are automatically visible in Gitbook as well.

## How to REVIEW a document?

When your document is ready for review, do the following:

1. On [Github](https://github.com/wri/.core-api), open a pull request for your `draft/` branch. Fill out the pull request form to document what kind of changes you have made and anything else you want reviewers to do.
2. Add reviewers to your PR.
   * If you are writing an ADR, the reviewers should the ADR's Deciders.
   * If you are writing an SDS, the reviewers should be the SDS's Reviewers.
3. Reviewers can then go over your document, and leave comments either directly in Gitbook or on the PR in Github.
4. Once all comments are resolved, the reviewers will approve the PR. After approval, you can merge your `draft/` branch into `master`. Your change will now be visible in the main version on Gitbook and you can delete the `draft/` branch.

