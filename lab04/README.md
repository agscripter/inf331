# Modelo para Apresentação do Lab04 - Serviços

Estrutura de pastas:

~~~
├── README.md  <- arquivo apresentando a tarefa
│
└── images     <- arquivos de imagens usadas no documento
~~~

## Tarefa 1
> Coloque a imagem do PNG do seu diagrama como ilustrado abaixo:
> 
> ![Diagrama de Orquestração](images/componentizacao-negocio.png)

## Tarefa 2
> Coloque a imagem do PNG do seu diagrama como ilustrado abaixo:
> 
> ![Diagrama de Orquestração](images/componentizacao-tecnico-view.png)

## Tarefa 3
> Coloque a imagem do PNG do seu diagrama como ilustrado abaixo:
> 
> ![Diagrama de Orquestração](images/componentizacao-tecnico-model.png)


## Tarefa 4

### Serviço `GitHub v3 API`

* **Título do serviço**: `Lista dee repositórios para um usuário`
* **Breve descrição**: 
  > A API retorna todos os repositórios para um usuário dado um nome de usuário: https://developer.github.com/v3/repos/#list-repositories-for-a-user
* **URL completa da requisição**: `https://api.github.com/users/agscripter/repos&sort=full_name`
* **Cabeçalho HTTP da chamada**:
~~~http
HTTP/1.1 200 OK
server: GitHub.com
date: Fri, 28 Aug 2020 00:23:51 GMT
content-type: application/json; charset=utf-8
status: 200 OK
cache-control: public, max-age=60, s-maxage=60
vary: Accept, Accept-Encoding, Accept, X-Requested-With
etag: W/"66152a87975079633ec7dc64520eedd1"
x-github-media-type: github.v3; format=json
access-control-expose-headers: ETag, Link, Location, Retry-After, X-GitHub-OTP, X-RateLimit-Limit, X-RateLimit-Remaining, X-RateLimit-Reset, X-OAuth-Scopes, X-Accepted-OAuth-Scopes, X-Poll-Interval, X-GitHub-Media-Type, Deprecation, Sunset
~~~
* **Cabeçalho HTTP da resposta**:
~~~http
access-control-allow-origin: *
strict-transport-security: max-age=31536000; includeSubdomains; preload
x-frame-options: deny
x-content-type-options: nosniff
x-xss-protection: 1; mode=block
referrer-policy: origin-when-cross-origin, strict-origin-when-cross-origin
content-security-policy: default-src 'none'
X-Ratelimit-Limit: 60
X-Ratelimit-Remaining: 54
X-Ratelimit-Reset: 1598575441
Accept-Ranges: bytes
Transfer-Encoding: chunked
X-GitHub-Request-Id: 218C:0EBC:FA9B15:1AB6AF5:5F484F43
~~~
* **Conteúdo da resposta**:
~~~json
[
  {
    "id": 256299378,
    "node_id": "MDEwOlJlcG9zaXRvcnkyNTYyOTkzNzg=",
    "name": "aws-lambda-cpp",
    "full_name": "agscripter/aws-lambda-cpp",
    "private": false,
    "owner": {
      "login": "agscripter",
      "id": 3118300,
      "node_id": "MDQ6VXNlcjMxMTgzMDA=",
      "avatar_url": "https://avatars3.githubusercontent.com/u/3118300?v=4",
      "gravatar_id": "",
      "url": "https://api.github.com/users/agscripter",
      "html_url": "https://github.com/agscripter",
      "followers_url": "https://api.github.com/users/agscripter/followers",
      "following_url": "https://api.github.com/users/agscripter/following{/other_user}",
      "gists_url": "https://api.github.com/users/agscripter/gists{/gist_id}",
      "starred_url": "https://api.github.com/users/agscripter/starred{/owner}{/repo}",
      "subscriptions_url": "https://api.github.com/users/agscripter/subscriptions",
      "organizations_url": "https://api.github.com/users/agscripter/orgs",
      "repos_url": "https://api.github.com/users/agscripter/repos",
      "events_url": "https://api.github.com/users/agscripter/events{/privacy}",
      "received_events_url": "https://api.github.com/users/agscripter/received_events",
      "type": "User",
      "site_admin": false
    },
    "html_url": "https://github.com/agscripter/aws-lambda-cpp",
    "description": "C++ implementation of the AWS Lambda runtime",
    "fork": true,
    "url": "https://api.github.com/repos/agscripter/aws-lambda-cpp",
    "forks_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/forks",
    "keys_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/keys{/key_id}",
    "collaborators_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/collaborators{/collaborator}",
    "teams_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/teams",
    "hooks_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/hooks",
    "issue_events_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/issues/events{/number}",
    "events_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/events",
    "assignees_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/assignees{/user}",
    "branches_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/branches{/branch}",
    "tags_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/tags",
    "blobs_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/git/blobs{/sha}",
    "git_tags_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/git/tags{/sha}",
    "git_refs_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/git/refs{/sha}",
    "trees_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/git/trees{/sha}",
    "statuses_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/statuses/{sha}",
    "languages_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/languages",
    "stargazers_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/stargazers",
    "contributors_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/contributors",
    "subscribers_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/subscribers",
    "subscription_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/subscription",
    "commits_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/commits{/sha}",
    "git_commits_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/git/commits{/sha}",
    "comments_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/comments{/number}",
    "issue_comment_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/issues/comments{/number}",
    "contents_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/contents/{+path}",
    "compare_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/compare/{base}...{head}",
    "merges_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/merges",
    "archive_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/{archive_format}{/ref}",
    "downloads_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/downloads",
    "issues_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/issues{/number}",
    "pulls_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/pulls{/number}",
    "milestones_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/milestones{/number}",
    "notifications_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/notifications{?since,all,participating}",
    "labels_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/labels{/name}",
    "releases_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/releases{/id}",
    "deployments_url": "https://api.github.com/repos/agscripter/aws-lambda-cpp/deployments",
    "created_at": "2020-04-16T18:37:58Z",
    "updated_at": "2020-04-17T14:06:07Z",
    "pushed_at": "2020-04-17T14:06:05Z",
    "git_url": "git://github.com/agscripter/aws-lambda-cpp.git",
    "ssh_url": "git@github.com:agscripter/aws-lambda-cpp.git",
    "clone_url": "https://github.com/agscripter/aws-lambda-cpp.git",
    "svn_url": "https://github.com/agscripter/aws-lambda-cpp",
    "homepage": "",
    "size": 431,
    "stargazers_count": 0,
    "watchers_count": 0,
    "language": "C++",
    "has_issues": false,
    "has_projects": true,
    "has_downloads": true,
    "has_wiki": false,
    "has_pages": false,
    "forks_count": 0,
    "mirror_url": null,
    "archived": false,
    "disabled": false,
    "open_issues_count": 0,
    "license": {
      "key": "apache-2.0",
      "name": "Apache License 2.0",
      "spdx_id": "Apache-2.0",
      "url": "https://api.github.com/licenses/apache-2.0",
      "node_id": "MDc6TGljZW5zZTI="
    },
    "forks": 0,
    "open_issues": 0,
    "watchers": 0,
    "default_branch": "master"
  },
  {
    "id": 244371148,
    "node_id": "MDEwOlJlcG9zaXRvcnkyNDQzNzExNDg=",
    "name": "cdk-deploying-lambda",
    "full_name": "agscripter/cdk-deploying-lambda",
    "private": false,
    "owner": {
      "login": "agscripter",
      "id": 3118300,
      "node_id": "MDQ6VXNlcjMxMTgzMDA=",
      "avatar_url": "https://avatars3.githubusercontent.com/u/3118300?v=4",
      "gravatar_id": "",
      "url": "https://api.github.com/users/agscripter",
      "html_url": "https://github.com/agscripter",
      "followers_url": "https://api.github.com/users/agscripter/followers",
      "following_url": "https://api.github.com/users/agscripter/following{/other_user}",
      "gists_url": "https://api.github.com/users/agscripter/gists{/gist_id}",
      "starred_url": "https://api.github.com/users/agscripter/starred{/owner}{/repo}",
      "subscriptions_url": "https://api.github.com/users/agscripter/subscriptions",
      "organizations_url": "https://api.github.com/users/agscripter/orgs",
      "repos_url": "https://api.github.com/users/agscripter/repos",
      "events_url": "https://api.github.com/users/agscripter/events{/privacy}",
      "received_events_url": "https://api.github.com/users/agscripter/received_events",
      "type": "User",
      "site_admin": false
    },
    "html_url": "https://github.com/agscripter/cdk-deploying-lambda",
    "description": null,
    "fork": false,
    "url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda",
    "forks_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/forks",
    "keys_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/keys{/key_id}",
    "collaborators_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/collaborators{/collaborator}",
    "teams_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/teams",
    "hooks_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/hooks",
    "issue_events_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/issues/events{/number}",
    "events_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/events",
    "assignees_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/assignees{/user}",
    "branches_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/branches{/branch}",
    "tags_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/tags",
    "blobs_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/git/blobs{/sha}",
    "git_tags_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/git/tags{/sha}",
    "git_refs_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/git/refs{/sha}",
    "trees_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/git/trees{/sha}",
    "statuses_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/statuses/{sha}",
    "languages_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/languages",
    "stargazers_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/stargazers",
    "contributors_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/contributors",
    "subscribers_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/subscribers",
    "subscription_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/subscription",
    "commits_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/commits{/sha}",
    "git_commits_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/git/commits{/sha}",
    "comments_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/comments{/number}",
    "issue_comment_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/issues/comments{/number}",
    "contents_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/contents/{+path}",
    "compare_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/compare/{base}...{head}",
    "merges_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/merges",
    "archive_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/{archive_format}{/ref}",
    "downloads_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/downloads",
    "issues_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/issues{/number}",
    "pulls_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/pulls{/number}",
    "milestones_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/milestones{/number}",
    "notifications_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/notifications{?since,all,participating}",
    "labels_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/labels{/name}",
    "releases_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/releases{/id}",
    "deployments_url": "https://api.github.com/repos/agscripter/cdk-deploying-lambda/deployments",
    "created_at": "2020-03-02T12:56:02Z",
    "updated_at": "2020-03-02T16:50:19Z",
    "pushed_at": "2020-03-02T16:50:16Z",
    "git_url": "git://github.com/agscripter/cdk-deploying-lambda.git",
    "ssh_url": "git@github.com:agscripter/cdk-deploying-lambda.git",
    "clone_url": "https://github.com/agscripter/cdk-deploying-lambda.git",
    "svn_url": "https://github.com/agscripter/cdk-deploying-lambda",
    "homepage": null,
    "size": 8,
    "stargazers_count": 0,
    "watchers_count": 0,
    "language": "Java",
    "has_issues": true,
    "has_projects": true,
    "has_downloads": true,
    "has_wiki": true,
    "has_pages": false,
    "forks_count": 0,
    "mirror_url": null,
    "archived": false,
    "disabled": false,
    "open_issues_count": 0,
    "license": null,
    "forks": 0,
    "open_issues": 0,
    "watchers": 0,
    "default_branch": "master"
  },
  {
    "id": 284837136,
    "node_id": "MDEwOlJlcG9zaXRvcnkyODQ4MzcxMzY=",
    "name": "inf331",
    "full_name": "agscripter/inf331",
    "private": false,
    "owner": {
      "login": "agscripter",
      "id": 3118300,
      "node_id": "MDQ6VXNlcjMxMTgzMDA=",
      "avatar_url": "https://avatars3.githubusercontent.com/u/3118300?v=4",
      "gravatar_id": "",
      "url": "https://api.github.com/users/agscripter",
      "html_url": "https://github.com/agscripter",
      "followers_url": "https://api.github.com/users/agscripter/followers",
      "following_url": "https://api.github.com/users/agscripter/following{/other_user}",
      "gists_url": "https://api.github.com/users/agscripter/gists{/gist_id}",
      "starred_url": "https://api.github.com/users/agscripter/starred{/owner}{/repo}",
      "subscriptions_url": "https://api.github.com/users/agscripter/subscriptions",
      "organizations_url": "https://api.github.com/users/agscripter/orgs",
      "repos_url": "https://api.github.com/users/agscripter/repos",
      "events_url": "https://api.github.com/users/agscripter/events{/privacy}",
      "received_events_url": "https://api.github.com/users/agscripter/received_events",
      "type": "User",
      "site_admin": false
    },
    "html_url": "https://github.com/agscripter/inf331",
    "description": null,
    "fork": false,
    "url": "https://api.github.com/repos/agscripter/inf331",
    "forks_url": "https://api.github.com/repos/agscripter/inf331/forks",
    "keys_url": "https://api.github.com/repos/agscripter/inf331/keys{/key_id}",
    "collaborators_url": "https://api.github.com/repos/agscripter/inf331/collaborators{/collaborator}",
    "teams_url": "https://api.github.com/repos/agscripter/inf331/teams",
    "hooks_url": "https://api.github.com/repos/agscripter/inf331/hooks",
    "issue_events_url": "https://api.github.com/repos/agscripter/inf331/issues/events{/number}",
    "events_url": "https://api.github.com/repos/agscripter/inf331/events",
    "assignees_url": "https://api.github.com/repos/agscripter/inf331/assignees{/user}",
    "branches_url": "https://api.github.com/repos/agscripter/inf331/branches{/branch}",
    "tags_url": "https://api.github.com/repos/agscripter/inf331/tags",
    "blobs_url": "https://api.github.com/repos/agscripter/inf331/git/blobs{/sha}",
    "git_tags_url": "https://api.github.com/repos/agscripter/inf331/git/tags{/sha}",
    "git_refs_url": "https://api.github.com/repos/agscripter/inf331/git/refs{/sha}",
    "trees_url": "https://api.github.com/repos/agscripter/inf331/git/trees{/sha}",
    "statuses_url": "https://api.github.com/repos/agscripter/inf331/statuses/{sha}",
    "languages_url": "https://api.github.com/repos/agscripter/inf331/languages",
    "stargazers_url": "https://api.github.com/repos/agscripter/inf331/stargazers",
    "contributors_url": "https://api.github.com/repos/agscripter/inf331/contributors",
    "subscribers_url": "https://api.github.com/repos/agscripter/inf331/subscribers",
    "subscription_url": "https://api.github.com/repos/agscripter/inf331/subscription",
    "commits_url": "https://api.github.com/repos/agscripter/inf331/commits{/sha}",
    "git_commits_url": "https://api.github.com/repos/agscripter/inf331/git/commits{/sha}",
    "comments_url": "https://api.github.com/repos/agscripter/inf331/comments{/number}",
    "issue_comment_url": "https://api.github.com/repos/agscripter/inf331/issues/comments{/number}",
    "contents_url": "https://api.github.com/repos/agscripter/inf331/contents/{+path}",
    "compare_url": "https://api.github.com/repos/agscripter/inf331/compare/{base}...{head}",
    "merges_url": "https://api.github.com/repos/agscripter/inf331/merges",
    "archive_url": "https://api.github.com/repos/agscripter/inf331/{archive_format}{/ref}",
    "downloads_url": "https://api.github.com/repos/agscripter/inf331/downloads",
    "issues_url": "https://api.github.com/repos/agscripter/inf331/issues{/number}",
    "pulls_url": "https://api.github.com/repos/agscripter/inf331/pulls{/number}",
    "milestones_url": "https://api.github.com/repos/agscripter/inf331/milestones{/number}",
    "notifications_url": "https://api.github.com/repos/agscripter/inf331/notifications{?since,all,participating}",
    "labels_url": "https://api.github.com/repos/agscripter/inf331/labels{/name}",
    "releases_url": "https://api.github.com/repos/agscripter/inf331/releases{/id}",
    "deployments_url": "https://api.github.com/repos/agscripter/inf331/deployments",
    "created_at": "2020-08-04T00:28:44Z",
    "updated_at": "2020-08-22T00:59:34Z",
    "pushed_at": "2020-08-22T00:59:32Z",
    "git_url": "git://github.com/agscripter/inf331.git",
    "ssh_url": "git@github.com:agscripter/inf331.git",
    "clone_url": "https://github.com/agscripter/inf331.git",
    "svn_url": "https://github.com/agscripter/inf331",
    "homepage": null,
    "size": 6719,
    "stargazers_count": 0,
    "watchers_count": 0,
    "language": "Jupyter Notebook",
    "has_issues": true,
    "has_projects": true,
    "has_downloads": true,
    "has_wiki": true,
    "has_pages": false,
    "forks_count": 0,
    "mirror_url": null,
    "archived": false,
    "disabled": false,
    "open_issues_count": 0,
    "license": null,
    "forks": 0,
    "open_issues": 0,
    "watchers": 0,
    "default_branch": "master"
  },
  {
    "id": 245895458,
    "node_id": "MDEwOlJlcG9zaXRvcnkyNDU4OTU0NTg=",
    "name": "Prototipo-IHC",
    "full_name": "agscripter/Prototipo-IHC",
    "private": false,
    "owner": {
      "login": "agscripter",
      "id": 3118300,
      "node_id": "MDQ6VXNlcjMxMTgzMDA=",
      "avatar_url": "https://avatars3.githubusercontent.com/u/3118300?v=4",
      "gravatar_id": "",
      "url": "https://api.github.com/users/agscripter",
      "html_url": "https://github.com/agscripter",
      "followers_url": "https://api.github.com/users/agscripter/followers",
      "following_url": "https://api.github.com/users/agscripter/following{/other_user}",
      "gists_url": "https://api.github.com/users/agscripter/gists{/gist_id}",
      "starred_url": "https://api.github.com/users/agscripter/starred{/owner}{/repo}",
      "subscriptions_url": "https://api.github.com/users/agscripter/subscriptions",
      "organizations_url": "https://api.github.com/users/agscripter/orgs",
      "repos_url": "https://api.github.com/users/agscripter/repos",
      "events_url": "https://api.github.com/users/agscripter/events{/privacy}",
      "received_events_url": "https://api.github.com/users/agscripter/received_events",
      "type": "User",
      "site_admin": false
    },
    "html_url": "https://github.com/agscripter/Prototipo-IHC",
    "description": "protótipo de ihc",
    "fork": true,
    "url": "https://api.github.com/repos/agscripter/Prototipo-IHC",
    "forks_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/forks",
    "keys_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/keys{/key_id}",
    "collaborators_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/collaborators{/collaborator}",
    "teams_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/teams",
    "hooks_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/hooks",
    "issue_events_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/issues/events{/number}",
    "events_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/events",
    "assignees_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/assignees{/user}",
    "branches_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/branches{/branch}",
    "tags_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/tags",
    "blobs_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/git/blobs{/sha}",
    "git_tags_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/git/tags{/sha}",
    "git_refs_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/git/refs{/sha}",
    "trees_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/git/trees{/sha}",
    "statuses_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/statuses/{sha}",
    "languages_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/languages",
    "stargazers_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/stargazers",
    "contributors_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/contributors",
    "subscribers_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/subscribers",
    "subscription_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/subscription",
    "commits_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/commits{/sha}",
    "git_commits_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/git/commits{/sha}",
    "comments_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/comments{/number}",
    "issue_comment_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/issues/comments{/number}",
    "contents_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/contents/{+path}",
    "compare_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/compare/{base}...{head}",
    "merges_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/merges",
    "archive_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/{archive_format}{/ref}",
    "downloads_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/downloads",
    "issues_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/issues{/number}",
    "pulls_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/pulls{/number}",
    "milestones_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/milestones{/number}",
    "notifications_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/notifications{?since,all,participating}",
    "labels_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/labels{/name}",
    "releases_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/releases{/id}",
    "deployments_url": "https://api.github.com/repos/agscripter/Prototipo-IHC/deployments",
    "created_at": "2020-03-08T22:07:00Z",
    "updated_at": "2020-03-08T22:09:09Z",
    "pushed_at": "2020-03-08T22:09:07Z",
    "git_url": "git://github.com/agscripter/Prototipo-IHC.git",
    "ssh_url": "git@github.com:agscripter/Prototipo-IHC.git",
    "clone_url": "https://github.com/agscripter/Prototipo-IHC.git",
    "svn_url": "https://github.com/agscripter/Prototipo-IHC",
    "homepage": null,
    "size": 261,
    "stargazers_count": 0,
    "watchers_count": 0,
    "language": "HTML",
    "has_issues": false,
    "has_projects": true,
    "has_downloads": true,
    "has_wiki": true,
    "has_pages": false,
    "forks_count": 0,
    "mirror_url": null,
    "archived": false,
    "disabled": false,
    "open_issues_count": 0,
    "license": {
      "key": "mit",
      "name": "MIT License",
      "spdx_id": "MIT",
      "url": "https://api.github.com/licenses/mit",
      "node_id": "MDc6TGljZW5zZTEz"
    },
    "forks": 0,
    "open_issues": 0,
    "watchers": 0,
    "default_branch": "master"
  },
  {
    "id": 121333450,
    "node_id": "MDEwOlJlcG9zaXRvcnkxMjEzMzM0NTA=",
    "name": "raml-tester",
    "full_name": "agscripter/raml-tester",
    "private": false,
    "owner": {
      "login": "agscripter",
      "id": 3118300,
      "node_id": "MDQ6VXNlcjMxMTgzMDA=",
      "avatar_url": "https://avatars3.githubusercontent.com/u/3118300?v=4",
      "gravatar_id": "",
      "url": "https://api.github.com/users/agscripter",
      "html_url": "https://github.com/agscripter",
      "followers_url": "https://api.github.com/users/agscripter/followers",
      "following_url": "https://api.github.com/users/agscripter/following{/other_user}",
      "gists_url": "https://api.github.com/users/agscripter/gists{/gist_id}",
      "starred_url": "https://api.github.com/users/agscripter/starred{/owner}{/repo}",
      "subscriptions_url": "https://api.github.com/users/agscripter/subscriptions",
      "organizations_url": "https://api.github.com/users/agscripter/orgs",
      "repos_url": "https://api.github.com/users/agscripter/repos",
      "events_url": "https://api.github.com/users/agscripter/events{/privacy}",
      "received_events_url": "https://api.github.com/users/agscripter/received_events",
      "type": "User",
      "site_admin": false
    },
    "html_url": "https://github.com/agscripter/raml-tester",
    "description": "Test if a request/response matches a given raml definition",
    "fork": true,
    "url": "https://api.github.com/repos/agscripter/raml-tester",
    "forks_url": "https://api.github.com/repos/agscripter/raml-tester/forks",
    "keys_url": "https://api.github.com/repos/agscripter/raml-tester/keys{/key_id}",
    "collaborators_url": "https://api.github.com/repos/agscripter/raml-tester/collaborators{/collaborator}",
    "teams_url": "https://api.github.com/repos/agscripter/raml-tester/teams",
    "hooks_url": "https://api.github.com/repos/agscripter/raml-tester/hooks",
    "issue_events_url": "https://api.github.com/repos/agscripter/raml-tester/issues/events{/number}",
    "events_url": "https://api.github.com/repos/agscripter/raml-tester/events",
    "assignees_url": "https://api.github.com/repos/agscripter/raml-tester/assignees{/user}",
    "branches_url": "https://api.github.com/repos/agscripter/raml-tester/branches{/branch}",
    "tags_url": "https://api.github.com/repos/agscripter/raml-tester/tags",
    "blobs_url": "https://api.github.com/repos/agscripter/raml-tester/git/blobs{/sha}",
    "git_tags_url": "https://api.github.com/repos/agscripter/raml-tester/git/tags{/sha}",
    "git_refs_url": "https://api.github.com/repos/agscripter/raml-tester/git/refs{/sha}",
    "trees_url": "https://api.github.com/repos/agscripter/raml-tester/git/trees{/sha}",
    "statuses_url": "https://api.github.com/repos/agscripter/raml-tester/statuses/{sha}",
    "languages_url": "https://api.github.com/repos/agscripter/raml-tester/languages",
    "stargazers_url": "https://api.github.com/repos/agscripter/raml-tester/stargazers",
    "contributors_url": "https://api.github.com/repos/agscripter/raml-tester/contributors",
    "subscribers_url": "https://api.github.com/repos/agscripter/raml-tester/subscribers",
    "subscription_url": "https://api.github.com/repos/agscripter/raml-tester/subscription",
    "commits_url": "https://api.github.com/repos/agscripter/raml-tester/commits{/sha}",
    "git_commits_url": "https://api.github.com/repos/agscripter/raml-tester/git/commits{/sha}",
    "comments_url": "https://api.github.com/repos/agscripter/raml-tester/comments{/number}",
    "issue_comment_url": "https://api.github.com/repos/agscripter/raml-tester/issues/comments{/number}",
    "contents_url": "https://api.github.com/repos/agscripter/raml-tester/contents/{+path}",
    "compare_url": "https://api.github.com/repos/agscripter/raml-tester/compare/{base}...{head}",
    "merges_url": "https://api.github.com/repos/agscripter/raml-tester/merges",
    "archive_url": "https://api.github.com/repos/agscripter/raml-tester/{archive_format}{/ref}",
    "downloads_url": "https://api.github.com/repos/agscripter/raml-tester/downloads",
    "issues_url": "https://api.github.com/repos/agscripter/raml-tester/issues{/number}",
    "pulls_url": "https://api.github.com/repos/agscripter/raml-tester/pulls{/number}",
    "milestones_url": "https://api.github.com/repos/agscripter/raml-tester/milestones{/number}",
    "notifications_url": "https://api.github.com/repos/agscripter/raml-tester/notifications{?since,all,participating}",
    "labels_url": "https://api.github.com/repos/agscripter/raml-tester/labels{/name}",
    "releases_url": "https://api.github.com/repos/agscripter/raml-tester/releases{/id}",
    "deployments_url": "https://api.github.com/repos/agscripter/raml-tester/deployments",
    "created_at": "2018-02-13T03:19:35Z",
    "updated_at": "2018-02-13T03:19:37Z",
    "pushed_at": "2017-06-02T13:41:07Z",
    "git_url": "git://github.com/agscripter/raml-tester.git",
    "ssh_url": "git@github.com:agscripter/raml-tester.git",
    "clone_url": "https://github.com/agscripter/raml-tester.git",
    "svn_url": "https://github.com/agscripter/raml-tester",
    "homepage": null,
    "size": 1179,
    "stargazers_count": 0,
    "watchers_count": 0,
    "language": "Java",
    "has_issues": false,
    "has_projects": true,
    "has_downloads": true,
    "has_wiki": true,
    "has_pages": false,
    "forks_count": 0,
    "mirror_url": null,
    "archived": false,
    "disabled": false,
    "open_issues_count": 0,
    "license": {
      "key": "apache-2.0",
      "name": "Apache License 2.0",
      "spdx_id": "Apache-2.0",
      "url": "https://api.github.com/licenses/apache-2.0",
      "node_id": "MDc6TGljZW5zZTI="
    },
    "forks": 0,
    "open_issues": 0,
    "watchers": 0,
    "default_branch": "master"
  }
]
~~~

