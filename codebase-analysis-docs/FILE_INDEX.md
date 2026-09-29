# Prioritized Source File Index

`HASH8` is the first eight hex characters of SHA-256 at documentation time. Paths are repository-relative. Recompute after edits; these are navigation anchors, not immutable IDs.

| # | Priority | Path | Type | Lines | HASH8 | Notes |
|---:|:---:|---|---|---:|---|---|
| 1 | + | `ecommerce-customer/package.json` | Config | 24 | `6e3b3b48` | Framework/dependency manifest |
| 2 | + | `ecommerce-customer/app/page.jsx` | UI | 214 | `3622e9a9` | Storefront/catalog entry |
| 3 | + | `ecommerce-customer/lib/store/AppProviders.jsx` | State | 863 | `266d078d` | Auth/cart orchestration |
| 4 | + | `ecommerce-customer/lib/guestCart.js` | State | 29 | `a3f8226b` | Guest cart persistence |
| 5 | ~ | `ecommerce-customer/lib/catalogCache.js` | Cache | 22 | `2e0aebda` | SPA product cache |
| 6 | ~ | `ecommerce-customer/lib/pricing.js` | Business logic | 69 | `9f1cccee` | Configurable totals; apparently unused |
| 7 | + | `ecommerce-customer/lib/supabaseServer.js` | Security/data | 55 | `d09bb702` | User/service Supabase clients |
| 8 | + | `ecommerce-customer/lib/razorpayServer.js` | Payments | 62 | `09faa392` | SDK and signature helpers |
| 9 | + | `ecommerce-customer/app/checkout/page.jsx` | UI | 180 | `2bc7ff47` | Checkout totals and address |
| 10 | + | `ecommerce-customer/components/checkout/RazorpayCheckoutButton.jsx` | UI/payments | 126 | `61a1d504` | Checkout callback |
| 11 | + | `ecommerce-customer/app/api/v1/orders/create/route.js` | API/payments | 169 | `b5f0d559` | Order snapshot and stock reservation |
| 12 | + | `ecommerce-customer/app/api/v1/payments/verify/route.js` | API/payments | 80 | `d5a7e3a3` | Current direct payment finalizer |
| 13 | + | `ecommerce-customer/app/api/v1/webhooks/razorpay/route.js` | API/payments | 205 | `df193b11` | Signed webhook/reconciliation |
| 14 | + | `ecommerce-customer/app/api/v1/orders/route.js` | API | 59 | `99240a8f` | Customer order list |
| 15 | + | `ecommerce-customer/app/api/v1/orders/[id]/route.js` | API | 36 | `d09183ec` | Customer order detail |
| 16 | + | `ecommerce-customer/app/api/v1/cart/items/route.js` | API | 142 | `18538309` | Persistent cart mutation |
| 17 | + | `ecommerce-customer/app/api/v1/cart/merge/route.js` | API | 85 | `c9bc7a94` | Guest cart merge |
| 18 | ~ | `ecommerce-customer/app/api/v1/addresses/route.js` | API | 100 | `8295d32d` | Address validation/ownership |
| 19 | + | `ecommerce-admin/package.json` | Config | 26 | `07fbb3c4` | Framework/dependency manifest |
| 20 | + | `ecommerce-admin/middleware.js` | Security/navigation | 29 | `19454d00` | Admin page presence guard |
| 21 | + | `ecommerce-admin/lib/supabaseClient.js` | Security/data | 21 | `63439cb4` | Service-role client |
| 22 | + | `ecommerce-admin/app/api/v1/admin/auth/google/route.js` | API/security | 117 | `7d78134d` | Google/admin allow-list login |
| 23 | + | `ecommerce-admin/app/api/v1/admin/auth/me/route.js` | API/security | 60 | `3729d5fd` | JWT and current admin check |
| 24 | + | `ecommerce-admin/app/api/v1/admin/dashboard/metrics/route.js` | API/business logic | 143 | `7a3b6e19` | KPI calculations |
| 25 | ~ | `ecommerce-admin/app/api/v1/admin/dashboard/export/route.js` | API | 69 | `7551a5d6` | CSV export |
| 26 | + | `ecommerce-admin/app/admin/dashboard/page.jsx` | UI | 146 | `a4b61ef0` | Dashboard ranges/display |
| 27 | + | `ecommerce-admin/app/admin/catalog/page.jsx` | UI | 316 | `1370c5f7` | Catalog workflow orchestration |
| 28 | + | `ecommerce-admin/app/admin/catalog/api.js` | API client | 148 | `4d086256` | Edge Function wrappers |
| 29 | ~ | `ecommerce-admin/app/admin/catalog/validation.js` | Validation | 70 | `5242e65e` | Client-side input validation |
| 30 | + | `supabase/migrations/001_schema.sql` | SQL/schema | 313 | `ee40a6af` | Base entities, checks, RLS |
| 31 | + | `supabase/migrations/002_triggers.sql` | SQL/security | 209 | `fd6b978d` | Trigger wiring and Vault secrets |
| 32 | + | `supabase/migrations/20260929052253_checkout_and_payment.sql` | SQL/payments | 378 | `66b7ffc9` | Finalizer and stock release |
| 33 | + | `supabase/migrations/20260929052739_catalog_management.sql` | SQL/catalog | 78 | `bbaf31e8` | Category policy and stock RPC |
| 34 | + | `supabase/migrations/20260929051207_approve_refund_restore.sql` | SQL/refunds | 46 | `eb3b5c85` | Approval and restock RPC |
| 35 | + | `supabase/functions/_shared/adminAuth.ts` | Edge/security | 52 | `dcdd6428` | Custom admin token guard |
| 36 | + | `supabase/functions/_shared/cors.ts` | Edge/security | 19 | `4d46e469` | Preflight/allowed headers |
| 37 | + | `supabase/functions/admin-catalog-products/index.ts` | Edge/API | 201 | `057c5a54` | Product CRUD/list |
| 38 | + | `supabase/functions/admin-catalog-stock/index.ts` | Edge/API | 88 | `d4b1f8c2` | Atomic stock adjustment |
| 39 | + | `supabase/functions/admin-categories/index.ts` | Edge/API | 165 | `3116f1bf` | Category lifecycle |
| 40 | ~ | `supabase/functions/admin-media-upload/index.ts` | Edge/storage | 101 | `73d23e3e` | Public image upload |
| 41 | ~ | `supabase/functions/order-confirmation/index.ts` | Edge/email | 63 | `b07a960b` | Order confirmation |
| 42 | ~ | `supabase/functions/delivered-review-request/index.ts` | Edge/cron | 53 | `38f596ed` | Delayed review email |
| 43 | + | `supabase/functions/refund-processed/index.ts` | Edge/refunds | 60 | `a0130054` | Refund email and restock |
| 44 | ~ | `supabase/functions/stripe-webhook/index.ts` | Edge/payments | 115 | `aaed25e4` | Additional Stripe path |
