# Comparing `tmp/variational-0.2.2.tar.gz` & `tmp/variational-0.3.0.tar.gz`

## Comparing `variational-0.2.2.tar` & `variational-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 variational-0.2.2/requirements-test.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 variational-0.2.2/requirements.txt
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 variational-0.2.2/tests/test_backoff.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 variational-0.2.2/tests/test_smoke.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 variational-0.2.2/variational/__init__.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 variational-0.2.2/variational/auth.py
--rw-r--r--   0        0        0     7624 2020-02-02 00:00:00.000000 variational-0.2.2/variational/client.py
--rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 variational-0.2.2/variational/models.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 variational-0.2.2/variational/paginate.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 variational-0.2.2/variational/wrappers.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 variational-0.2.2/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 variational-0.2.2/LICENSE
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 variational-0.2.2/README.md
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 variational-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 variational-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 variational-0.3.0/requirements-test.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 variational-0.3.0/requirements.txt
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 variational-0.3.0/tests/test_backoff.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 variational-0.3.0/tests/test_smoke.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 variational-0.3.0/variational/__init__.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 variational-0.3.0/variational/auth.py
+-rw-r--r--   0        0        0    14544 2020-02-02 00:00:00.000000 variational-0.3.0/variational/client.py
+-rw-r--r--   0        0        0    13264 2020-02-02 00:00:00.000000 variational-0.3.0/variational/models.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 variational-0.3.0/variational/paginate.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 variational-0.3.0/variational/wrappers.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 variational-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 variational-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 variational-0.3.0/README.md
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 variational-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 variational-0.3.0/PKG-INFO
```

### Comparing `variational-0.2.2/variational/auth.py` & `variational-0.3.0/variational/auth.py`

 * *Files identical despite different names*

### Comparing `variational-0.2.2/variational/models.py` & `variational-0.3.0/variational/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,432 +1,516 @@
-import sys
-from enum import Enum
-from typing import TypedDict, Optional, List, Dict, Union
-
-if sys.version_info[0:2] >= (3, 10):
-    from typing import TypeAlias
-
-    DateTimeRFC3339: TypeAlias = str  # e.g. "2024-02-02T06:13:45.323432Z"
-    H160: TypeAlias = str  # e.g. "0x3d68316712565ccb7f14a2bfc6aa785d6d2d12d5"
-    UUIDv4: TypeAlias = str  # e.g. "bdd68c99-65fe-4500-baae-5bc09b4af183"
-    StrDecimal: TypeAlias = str  # e.g. "218205.58082"
-    AssetToken: TypeAlias = str  # e.g. "BTC", "ETH", etc
-else:
-    DateTimeRFC3339 = str
-    H160 = str
-    UUIDv4 = str
-    StrDecimal = str
-    AssetToken = str
+from enum import StrEnum
+from typing import TypeAlias, TypedDict, Optional, Union, Dict, List
 
+AssetToken: TypeAlias = str  # e.g. "BTC", "ETH", etc
+DateTimeRFC3339: TypeAlias = str  # e.g. "2024-02-02T06:13:45.323432Z"
+H160: TypeAlias = str  # e.g. "0x3d68316712565ccb7f14a2bfc6aa785d6d2d12d5"
+StrDecimal: TypeAlias = str  # e.g. "218205.58082"
+UUIDv4: TypeAlias = str  # e.g. "bdd68c99-65fe-4500-baae-5bc09b4af183"
 
-class Address(TypedDict):
-    created_at: Optional[DateTimeRFC3339]
-    company: UUIDv4
-    address: H160
-    enabled: bool
 
+# Enums
 
-class Company(TypedDict):
-    id: UUIDv4
-    created_at: Optional[DateTimeRFC3339]
-    legal_name: str
-    short_name: str
-    is_lp: bool
+class ApiRole(StrEnum):
+    READER = "reader"
+    WRITER = "writer"
 
 
-class Asset(TypedDict):
-    company: UUIDv4
-    pool_location: UUIDv4
-    asset: AssetToken
-    qty: StrDecimal
+class ClearingStatus(StrEnum):
+    PENDING_TAKER_DEPOSIT_APPROVAL = "pending_taker_deposit_approval"
+    PENDING_MAKER_DEPOSIT_APPROVAL = "pending_maker_deposit_approval"
+    PENDING_MAKER_LAST_LOOK = "pending_maker_last_look"
+    PENDING_POOL_CREATION = "pending_pool_creation"
+    PENDING_ATOMIC_DEPOSIT = "pending_atomic_deposit"
+    REJECTED_FAILED_TAKER_DEPOSIT_APPROVAL = "rejected_failed_taker_deposit_approval"
+    REJECTED_FAILED_MAKER_DEPOSIT_APPROVAL = "rejected_failed_maker_deposit_approval"
+    REJECTED_MAKER_LAST_LOOK_REJECTED = "rejected_maker_last_look_rejected"
+    REJECTED_MAKER_LAST_LOOK_EXPIRED = "rejected_maker_last_look_expired"
+    REJECTED_FAILED_POOL_CREATION = "rejected_failed_pool_creation"
+    REJECTED_FAILED_TAKER_FUNDING = "rejected_failed_taker_funding"
+    REJECTED_FAILED_MAKER_FUNDING = "rejected_failed_maker_funding"
+    REJECTED_FAILED_ATOMIC_DEPOSIT = "rejected_failed_atomic_deposit"
+    SUCCESS_TRADES_BOOKED_INTO_POOL = "success_trades_booked_into_pool"
 
 
-class InstrumentType(Enum):
-    SPOT = "spot"
-    DATED_FUTURE = "dated_future"
-    PERPETUAL_FUTURE = "perpetual_future"
-    VANILLA_OPTION = "vanilla_option"
+class DexNetworkID(StrEnum):
+    ETH = "eth"
+    BSC = "bsc"
+    SOLANA = "solana"
 
 
-class Spot(TypedDict):
-    instrument_type: InstrumentType  # == SPOT
-    underlying: str
-    settlement_asset: str
+class ExerciseType(StrEnum):
+    EUROPEAN = "european"
+    AMERICAN = "american"
 
 
-class DatedFuture(TypedDict):
-    instrument_type: InstrumentType  # == DATED_FUTURE
-    underlying: str
-    settlement_asset: str
-    expiry: DateTimeRFC3339
+class InstrumentType(StrEnum):
+    SPOT = "spot"
+    DATED_FUTURE = "dated_future"
+    PERPETUAL_FUTURE = "perpetual_future"
+    VANILLA_OPTION = "vanilla_option"
 
 
-class PerpetualFuture(TypedDict):
-    instrument_type: InstrumentType  # == PERPETUAL_FUTURE
-    underlying: str
-    settlement_asset: str
-    funding_interval_s: int
+class MarginMode(StrEnum):
+    SIMPLE = "simple"
+    PORTFOLIO = "portfolio"
 
 
-class PayoffType(Enum):
+class PayoffType(StrEnum):
     PUT = "put"
     CALL = "call"
 
 
-class ExerciseType(Enum):
-    EUROPEAN = "european"
-    AMERICAN = "american"
+class PoolStrategyType(StrEnum):
+    USE_EXISTING = "use_existing"
+    CREATE_NEW = "create_new"
 
 
-class VanillaOption(TypedDict):
-    instrument_type: InstrumentType  # == VANILLA_OPTION
-    underlying: str
-    settlement_asset: str
-    expiry: DateTimeRFC3339
-    strike: StrDecimal
-    payoff: PayoffType
-    exercise: ExerciseType
+class RFQStatus(StrEnum):
+    OPEN = "open"
+    EXPIRED = "expired"
+    CANCELED = "canceled"
+    CLOSED = "closed"
 
 
-Instrument = Union[Spot, DatedFuture, PerpetualFuture, VanillaOption]
+class RequestAction(StrEnum):
+    REJECT = "reject"
+    ACCEPT = "accept"
 
 
-class Position(TypedDict):
-    company: UUIDv4
-    pool_location: UUIDv4
-    instrument: Instrument
-    updated_at: Optional[DateTimeRFC3339]
-    qty: StrDecimal
-    avg_entry_price: StrDecimal
+class SettlementPoolStatus(StrEnum):
+    OPEN = "open"
+    PENDING = "pending"
+    CANCELED = "canceled"
 
 
-class AggregatedPosition(TypedDict):
-    price: StrDecimal
-    underlying_price: StrDecimal
-    iv: StrDecimal
-    sum_delta: StrDecimal
-    sum_gamma: StrDecimal
-    upnl: StrDecimal
-    notional: StrDecimal
-    sum_rho: StrDecimal
-    sum_theta: StrDecimal
-    sum_vega: StrDecimal
-    position_info: Position
+class TradeRole(StrEnum):
+    MAKER = "maker"
+    TAKER = "taker"
 
 
-class TradeSide(Enum):
+class TradeSide(StrEnum):
     BUY = "buy"
     SELL = "sell"
 
 
-class TradeRole(Enum):
-    MAKER = "maker"
-    TAKER = "taker"
-
-
-class TradeType(Enum):
+class TradeType(StrEnum):
     TRADE = "trade"
     SETTLEMENT = "settlement"
     LIQUIDATION = "liquidation"
 
 
-class Trade(TypedDict):
-    id: UUIDv4
-    source_rfq: Optional[UUIDv4]
-    source_rfq_leg_id: Optional[UUIDv4]
-    source_quote: Optional[UUIDv4]
-    company: UUIDv4
-    created_at: Optional[DateTimeRFC3339]
-    side: TradeSide
-    instrument: Instrument
-    price: StrDecimal
-    qty: StrDecimal
-    pool_location: UUIDv4
-    role: TradeRole
-    trade_type: TradeType
+class TransferStatus(StrEnum):
+    PENDING = "pending"
+    FAILED = "failed"
+    CONFIRMED = "confirmed"
 
 
-class SimpleMarginAssetParam(TypedDict):
-    futures_initial_margin: StrDecimal
-    futures_maintenance_margin: StrDecimal
-    futures_leverage: StrDecimal
-    option_initial_margin: StrDecimal
-    option_initial_margin_min: StrDecimal
-    option_maintenance_margin: StrDecimal
+class TransferType(StrEnum):
+    PREMIUM = "premium"
+    DEPOSIT = "deposit"
+    WITHDRAWAL = "withdrawal"
+    SETTLEMENT = "settlement"
+    LIQUIDATION = "liquidation"
+    REALIZED_PNL = "realized_pnl"
+    INITIAL_MARGIN = "initial_margin"
 
 
-class MarginMode(Enum):
-    SIMPLE = "simple"
-    PORTFOLIO = "portfolio"
+# Nested models
 
+class ClearingEvent(TypedDict):
+    rfq_id: UUIDv4
+    parent_quote_id: UUIDv4
+    status: ClearingStatus
+    created_at: DateTimeRFC3339
+    taker_side: Optional[TradeSide]
 
-class SimpleMarginParams(TypedDict):
-    margin_mode: MarginMode  # == SIMPLE
-    asset_params: Dict[AssetToken, SimpleMarginAssetParam]
-    liquidation_penalty: StrDecimal
-    auto_liquidation: bool
 
+class CreateNewPool(TypedDict):
+    strategy: PoolStrategyType  # = CREATE_NEW
+    name: str  # length ∈ [1, 50]
+    creator_params: 'MarginParams'
+    other_params: 'MarginParams'
 
-class PortfolioMarginAssetParam(TypedDict):
-    vol_range_up: StrDecimal
-    vol_range_down: StrDecimal
-    short_vega_power: StrDecimal
-    long_vega_power: StrDecimal
-    price_range: StrDecimal
-    opt_sum_contingency: StrDecimal
-    opt_contingency: StrDecimal
-    futures_contingency: StrDecimal
-    atm_range: StrDecimal
 
+class DatedFuture(TypedDict):
+    instrument_type: InstrumentType  # = DATED_FUTURE
+    underlying: str  # ∈ {'BTC', 'ETH'}
+    settlement_asset: str  # = 'USDC'
+    expiry: DateTimeRFC3339  # date in the future or datetime at 08:00:00Z
 
-class PortfolioMarginParams(TypedDict):
-    margin_mode: MarginMode  # == PORTFOLIO
-    asset_params: Dict[AssetToken, PortfolioMarginAssetParam]
-    decorrelation_risk: StrDecimal
-    initial_margin_factor: StrDecimal
-    liquidation_penalty: StrDecimal
-    auto_liquidation: bool
 
+class DexTokenDetails(TypedDict):
+    network: DexNetworkID
+    underlying_address: H160
 
-MarginParams = Union[SimpleMarginParams, PortfolioMarginParams]
+
+class FundingRateParams(TypedDict):
+    normal_threshold: StrDecimal
+    high_threshold: StrDecimal
+    extreme_threshold: StrDecimal
+    normal_slope: StrDecimal
+    high_slope: StrDecimal
+    extreme_slope: StrDecimal
+    min_imbalance_dollars: StrDecimal
+    funding_exponent_factor: StrDecimal
+
+
+class Leg(TypedDict):
+    side: TradeSide
+    ratio: int  # ≥ 1
+    instrument: 'Instrument'
 
 
 class MarginUsage(TypedDict):
     initial_margin: StrDecimal
     maintenance_margin: StrDecimal
 
 
+class PerpetualFuture(TypedDict):
+    instrument_type: InstrumentType  # = PERPETUAL_FUTURE
+    underlying: str
+    settlement_asset: str  # = 'USDC'
+    funding_interval_s: int  # = 3600
+    dex_token_details: Optional[DexTokenDetails]  # required if underlying is a DEX token
+
+
 class PoolMarginUsageStats(TypedDict):
     company: UUIDv4
     balance: StrDecimal
-    margin_params: MarginParams
+    margin_params: 'MarginParams'
     margin_usage: MarginUsage
 
 
-class SettlementPoolStatus(Enum):
-    OPEN = "open"
-    PENDING = "pending"
-    CANCELED = "canceled"
+class PortfolioMarginAssetParam(TypedDict):
+    vol_range_up: StrDecimal  # ∈ [0, 1]
+    vol_range_down: StrDecimal  # ∈ [0, 1]
+    short_vega_power: StrDecimal  # ∈ [0, 1]
+    long_vega_power: StrDecimal  # ∈ [0, 1]
+    price_range: StrDecimal  # ∈ [0, 1]
+    opt_sum_contingency: StrDecimal  # ∈ [0, 1]
+    opt_contingency: StrDecimal  # ∈ [0, 1]
+    futures_contingency: StrDecimal  # ∈ [0, 1]
+    atm_range: StrDecimal  # ∈ [0, 1]
+
+
+class PortfolioMarginParams(TypedDict):
+    asset_params: Dict[AssetToken, PortfolioMarginAssetParam]
+    default_asset_param: PortfolioMarginAssetParam
+    decorrelation_risk: StrDecimal  # ∈ [0, 1]
+    initial_margin_factor: StrDecimal  # > 1
+    liquidation_penalty: StrDecimal  # ∈ [0, 1]
+    auto_liquidation: bool
+
+
+class PortfolioMarginParamsTag(TypedDict):
+    margin_mode: MarginMode  # = PORTFOLIO
+    params: PortfolioMarginParams
+
+
+class QuoteCommonMetadata(TypedDict):
+    parent_quote_id: UUIDv4
+    maker_company: UUIDv4
+    clearing_status: Optional[ClearingStatus]
+    expires_at: DateTimeRFC3339
+    pool_location: Optional[UUIDv4]
+    new_pool_name: Optional[str]
+    creator_params: Optional['MarginParams']
+    other_params: Optional['MarginParams']
+    pool_creator_company: Optional[UUIDv4]
+    pool_other_company: Optional[UUIDv4]
+    pool_creator_params: Optional['MarginParams']
+    pool_other_params: Optional['MarginParams']
+    clearing_events: List[ClearingEvent]
+
+
+class QuoteWithMarginRequirements(TypedDict):
+    parent_quote_id: UUIDv4
+    quote_price: StrDecimal
+    counter_factual_margin_requirements: Optional[MarginUsage]
+    existing_margin_requirements: Optional[MarginUsage]
+    additional_margin_requirements: Optional[MarginUsage]
+    margin_requirements_counter_factual_request_id: UUIDv4
+    existing_margin_requirements_request_id: UUIDv4
+
+
+class RFQLeg(TypedDict):
+    rfq_leg_id: UUIDv4
+    rfq_id: UUIDv4
+    instrument: 'Instrument'
+    side: TradeSide
+    qty: StrDecimal
 
 
 class SettlementPoolData(TypedDict):
     status: SettlementPoolStatus
     pool_name: str
     pool_address: Optional[H160]
     creator_address: H160
     other_address: H160
-    positions: List[AggregatedPosition]
+    positions: List['AggregatedPosition']
     creator_company_margin_usage: PoolMarginUsageStats
     other_company_margin_usage: PoolMarginUsageStats
 
 
-class SettlementPool(TypedDict):
-    pool_id: UUIDv4
-    company_id: UUIDv4
-    data: Optional[SettlementPoolData]
-    error: Optional[str]
+class SimpleMarginAssetParam(TypedDict):
+    futures_initial_margin: StrDecimal  # ∈ [0, 1]
+    futures_maintenance_margin: StrDecimal  # ∈ [0, 1]
+    futures_leverage: StrDecimal  # > 0
+    option_initial_margin: StrDecimal  # ∈ [0, 1]
+    option_initial_margin_min: StrDecimal  # ∈ [0, 1]
+    option_maintenance_margin: StrDecimal  # ∈ [0, 1]
 
 
-class TransferStatus(Enum):
-    PENDING = "pending"
-    FAILED = "failed"
-    CONFIRMED = "confirmed"
+class SimpleMarginParams(TypedDict):
+    asset_params: Dict[AssetToken, SimpleMarginAssetParam]
+    default_asset_param: SimpleMarginAssetParam
+    liquidation_penalty: StrDecimal  # ∈ [0, 1]
+    auto_liquidation: bool
 
 
-class TransferType(Enum):
-    PREMIUM = "premium"
-    DEPOSIT = "deposit"
-    WITHDRAWAL = "withdrawal"
-    SETTLEMENT = "settlement"
-    LIQUIDATION = "liquidation"
-    REALIZED_PNL = "realized_pnl"
-    INITIAL_MARGIN = "initial_margin"
+class SimpleMarginParamsTag(TypedDict):
+    margin_mode: MarginMode  # = SIMPLE
+    params: SimpleMarginParams
 
 
-class Transfer(TypedDict):
-    id: UUIDv4
-    rfq_id: Optional[UUIDv4]
-    parent_quote_id: Optional[UUIDv4]
-    oracle_request_id: Optional[UUIDv4]
-    created_at: DateTimeRFC3339
+class Spot(TypedDict):
+    instrument_type: InstrumentType  # = SPOT
+    underlying: str
+    settlement_asset: str  # = 'USDC'
+
+
+class StructurePrice(TypedDict):
+    price: StrDecimal
+    native_price: StrDecimal
+    delta: StrDecimal
+    gamma: StrDecimal
+    theta: StrDecimal
+    vega: StrDecimal
+    rho: StrDecimal
+    timestamp: DateTimeRFC3339
+
+
+class UseExistingPool(TypedDict):
+    strategy: PoolStrategyType  # = USE_EXISTING
+    pool_id: UUIDv4
+
+
+class VanillaOption(TypedDict):
+    instrument_type: InstrumentType  # = VANILLA_OPTION
+    underlying: str  # ∈ {'BTC', 'ETH'}
+    settlement_asset: str  # = 'USDC'
+    expiry: DateTimeRFC3339  # date in the future or datetime at 08:00:00Z
+    strike: StrDecimal  # > 0
+    payoff: PayoffType
+    exercise: ExerciseType
+
+
+# Top-level models
+
+class Address(TypedDict):
+    created_at: Optional[DateTimeRFC3339]
     company: UUIDv4
-    qty: StrDecimal
-    asset: AssetToken
-    target_pool_location: UUIDv4
-    transfer_type: TransferType
-    status: TransferStatus
+    address: H160
+    enabled: bool
 
 
-class PortfolioSummary(TypedDict):
-    sum_balance: StrDecimal
+class AggregatedPosition(TypedDict):
+    price: StrDecimal
+    underlying_price: StrDecimal
+    iv: StrDecimal
     sum_delta: StrDecimal
     sum_gamma: StrDecimal
-    sum_upnl: StrDecimal
-    sum_notional: StrDecimal
+    upnl: StrDecimal
+    notional: StrDecimal
     sum_rho: StrDecimal
     sum_theta: StrDecimal
     sum_vega: StrDecimal
-    sum_dollar_delta: StrDecimal
-    sum_dollar_gamma: StrDecimal
+    position_info: 'Position'
 
 
-class ClearingStatus(Enum):
-    PENDING_TAKER_DEPOSIT_APPROVAL = "pending_taker_deposit_approval"
-    PENDING_MAKER_DEPOSIT_APPROVAL = "pending_maker_deposit_approval"
-    PENDING_MAKER_LAST_LOOK = "pending_maker_last_look"
-    PENDING_POOL_CREATION = "pending_pool_creation"
-    PENDING_ATOMIC_DEPOSIT = "pending_atomic_deposit"
-    REJECTED_FAILED_TAKER_DEPOSIT_APPROVAL = "rejected_failed_taker_deposit_approval"
-    REJECTED_FAILED_MAKER_DEPOSIT_APPROVAL = "rejected_failed_maker_deposit_approval"
-    REJECTED_MAKER_LAST_LOOK_REJECTED = "rejected_maker_last_look_rejected"
-    REJECTED_MAKER_LAST_LOOK_EXPIRED = "rejected_maker_last_look_expired"
-    REJECTED_FAILED_POOL_CREATION = "rejected_failed_pool_creation"
-    REJECTED_FAILED_TAKER_FUNDING = "rejected_failed_taker_funding"
-    REJECTED_FAILED_MAKER_FUNDING = "rejected_failed_maker_funding"
-    REJECTED_FAILED_ATOMIC_DEPOSIT = "rejected_failed_atomic_deposit"
-    SUCCESS_TRADES_BOOKED_INTO_POOL = "success_trades_booked_into_pool"
+class Asset(TypedDict):
+    company: UUIDv4
+    pool_location: UUIDv4
+    asset: AssetToken
+    qty: StrDecimal
 
 
-class ClearingEvent(TypedDict):
+class AtomicDepositDetails(TypedDict):
     rfq_id: UUIDv4
     parent_quote_id: UUIDv4
-    status: ClearingStatus
-    created_at: DateTimeRFC3339
-    taker_side: Optional[TradeSide]
-
-
-class LegQuote(TypedDict):
-    parent_quote_id: UUIDv4
-    quote_id: UUIDv4
-    target_rfq_leg_id: UUIDv4
-    ask: Optional[StrDecimal]
-    bid: Optional[StrDecimal]
+    pool_address: H160
+    creator_address: H160
+    creator_transfer_amount: StrDecimal
+    other_address: H160
+    other_transfer_amount: StrDecimal
 
 
-class Quote(TypedDict):
-    parent_quote_id: UUIDv4
-    target_rfq_id: UUIDv4
-    maker_company: UUIDv4
-    expires_at: DateTimeRFC3339
-    aggregated_bid: Optional[StrDecimal]
-    aggregated_ask: Optional[StrDecimal]
-    clearing_status: ClearingStatus
-    clearing_events: List[ClearingEvent]
-    new_pool_name: Optional[str]
-    creator_params: Optional[MarginParams]
-    other_params: Optional[MarginParams]
-    pool_location: Optional[UUIDv4]
-    per_leg_quotes: List[LegQuote]
+class AuthContext(TypedDict):
+    key_id: UUIDv4
+    company_id: UUIDv4
+    role: ApiRole
 
 
-class Leg(TypedDict):
-    side: TradeSide
-    ratio: int
-    instrument: Instrument
+class Company(TypedDict):
+    id: UUIDv4
+    created_at: Optional[DateTimeRFC3339]
+    legal_name: str
+    short_name: str
+    is_lp: bool
 
 
-class Structure(TypedDict):
-    legs: List[Leg]
+Instrument = Union[Spot, DatedFuture, PerpetualFuture, VanillaOption]
 
 
-class StructurePrice(TypedDict):
+class InstrumentPrice(TypedDict):
     price: StrDecimal
     native_price: StrDecimal
     delta: StrDecimal
     gamma: StrDecimal
     theta: StrDecimal
     vega: StrDecimal
     rho: StrDecimal
+    iv: StrDecimal
+    underlying_price: StrDecimal
+    interest_rate: StrDecimal
     timestamp: DateTimeRFC3339
 
 
-class RFQLeg(TypedDict):
-    rfq_leg_id: UUIDv4
-    rfq_id: UUIDv4
+class LegQuote(TypedDict):
+    target_rfq_leg_id: UUIDv4
+    ask: Optional[StrDecimal]  # > 0
+    bid: Optional[StrDecimal]  # > 0
+
+
+class MakerLastLookResponse(TypedDict):
+    new_clearing_status: ClearingStatus
+    pending_deposits_sum_qty: StrDecimal
+    atomic_deposit_details: Optional[AtomicDepositDetails]
+
+
+MarginParams = Union[SimpleMarginParamsTag, PortfolioMarginParamsTag]
+
+
+PoolStrategy = Union[UseExistingPool, CreateNewPool]
+
+
+class PortfolioSummary(TypedDict):
+    sum_balance: StrDecimal
+    sum_delta: StrDecimal
+    sum_gamma: StrDecimal
+    sum_upnl: StrDecimal
+    sum_notional: StrDecimal
+    sum_rho: StrDecimal
+    sum_theta: StrDecimal
+    sum_vega: StrDecimal
+    sum_dollar_delta: StrDecimal
+    sum_dollar_gamma: StrDecimal
+
+
+class Position(TypedDict):
+    company: UUIDv4
+    pool_location: UUIDv4
     instrument: Instrument
-    side: TradeSide
+    updated_at: Optional[DateTimeRFC3339]
     qty: StrDecimal
+    avg_entry_price: StrDecimal
 
 
-class QuoteCommonMetadata(TypedDict):
+class Quote(TypedDict):
     parent_quote_id: UUIDv4
+    target_rfq_id: UUIDv4
     maker_company: UUIDv4
-    clearing_status: Optional[ClearingStatus]
     expires_at: DateTimeRFC3339
-    pool_location: Optional[UUIDv4]
+    aggregated_bid: Optional[StrDecimal]
+    aggregated_ask: Optional[StrDecimal]
+    clearing_status: ClearingStatus
+    clearing_events: List[ClearingEvent]
     new_pool_name: Optional[str]
     creator_params: Optional[MarginParams]
     other_params: Optional[MarginParams]
-    pool_creator_company: Optional[UUIDv4]
-    pool_other_company: Optional[UUIDv4]
-    pool_creator_params: Optional[MarginParams]
-    pool_other_params: Optional[MarginParams]
-    clearing_events: List[ClearingEvent]
-
-
-class QuoteWithMarginRequirements(TypedDict):
-    parent_quote_id: UUIDv4
-    quote_price: StrDecimal
-    counter_factual_margin_requirements: Optional[MarginUsage]
-    existing_margin_requirements: Optional[MarginUsage]
-    additional_margin_requirements: Optional[MarginUsage]
-    margin_requirements_counter_factual_request_id: UUIDv4
-    existing_margin_requirements_request_id: UUIDv4
+    pool_location: Optional[UUIDv4]
+    per_leg_quotes: List[LegQuote]
 
 
-class RFQStatus(Enum):
-    OPEN = "open"
-    EXPIRED = "expired"
-    CANCELED = "canceled"
-    CLOSED = "closed"
+class QuoteAcceptResponse(TypedDict):
+    pending_deposits_sum_qty: StrDecimal
+    pending_settlement_pool: Optional['SettlementPool']
+    new_clearing_status: ClearingStatus
 
 
 class RFQ(TypedDict):
     rfq_id: UUIDv4
     created_at: DateTimeRFC3339
-    structure: Structure
+    clearing_status: Optional[ClearingStatus]
+    structure: 'Structure'
     structure_price: Optional[StructurePrice]
     rfq_expires_at: DateTimeRFC3339
     taker_company: UUIDv4
     rfq_status: RFQStatus
     qty: StrDecimal
     rfq_legs: List[RFQLeg]
     quotes_common_metadata: Dict[UUIDv4, QuoteCommonMetadata]
     bids: List[QuoteWithMarginRequirements]
     asks: List[QuoteWithMarginRequirements]
 
 
-class FundingRateParams(TypedDict):
-    normal_threshold: StrDecimal
-    high_threshold: StrDecimal
-    extreme_threshold: StrDecimal
-    normal_slope: StrDecimal
-    high_slope: StrDecimal
-    extreme_slope: StrDecimal
-    min_imbalance_dollars: StrDecimal
+class SettlementPool(TypedDict):
+    pool_id: UUIDv4
+    company_id: UUIDv4
+    data: Optional[SettlementPoolData]
+    error: Optional[str]
+
+
+class Status(TypedDict):
+    auth: Optional[AuthContext]
+    server_timestamp_ms: int
+
+
+class Structure(TypedDict):
+    legs: List[Leg]
+
+
+class StructurePriceResponse(TypedDict):
+    legs: List[InstrumentPrice]
+    structure: StructurePrice
 
 
 class SupportedAssetDetails(TypedDict):
     asset: AssetToken
     asset_name: str
     is_dex: bool
     address: Optional[H160]
     verified: Optional[bool]
     precision: int
     last_updated_at: DateTimeRFC3339
     variational_funding_rate_params: FundingRateParams
 
 
-class ApiRole(Enum):
-    READER = "reader"
-    WRITER = "writer"
-
-
-class AuthContext(TypedDict):
-    key_id: UUIDv4
-    company_id: UUIDv4
-    role: ApiRole
+class Trade(TypedDict):
+    id: UUIDv4
+    source_rfq: Optional[UUIDv4]
+    source_rfq_leg_id: Optional[UUIDv4]
+    source_quote: Optional[UUIDv4]
+    company: UUIDv4
+    created_at: Optional[DateTimeRFC3339]
+    side: TradeSide
+    instrument: Instrument
+    price: StrDecimal
+    qty: StrDecimal
+    pool_location: UUIDv4
+    role: TradeRole
+    trade_type: TradeType
 
 
-class Status(TypedDict):
-    auth: Optional[AuthContext]
-    server_timestamp_ms: int
+class Transfer(TypedDict):
+    id: UUIDv4
+    rfq_id: Optional[UUIDv4]
+    parent_quote_id: Optional[UUIDv4]
+    oracle_request_id: Optional[UUIDv4]
+    created_at: DateTimeRFC3339
+    company: UUIDv4
+    qty: StrDecimal
+    asset: AssetToken
+    target_pool_location: UUIDv4
+    transfer_type: TransferType
+    status: TransferStatus
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `variational-0.2.2/variational/paginate.py` & `variational-0.3.0/variational/paginate.py`

 * *Files identical despite different names*

### Comparing `variational-0.2.2/variational/wrappers.py` & `variational-0.3.0/variational/wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 class ResponseMetadata:
     # timestamp in seconds when API server received the request
     request_received_at: float
 
 
 @dataclass
 class ApiError(Exception):
+    url: str
     status_code: int
     api_code: int
     message: str
 
     def __str__(self):
         return repr(self)
```

### Comparing `variational-0.2.2/LICENSE` & `variational-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `variational-0.2.2/README.md` & `variational-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `variational-0.2.2/pyproject.toml` & `variational-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "variational"
-version = "0.2.2"
+version = "0.3.0"
 authors = [
   { name="Variational Research", email="hello@variational.io" },
 ]
 dependencies = [
     "requests >= 2.12",
     "Brotli >= 1.0",
 ]
 description = "Variational Reference SDK"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Financial and Insurance Industry",
     "Intended Audience :: Developers",
 ]
```

### Comparing `variational-0.2.2/PKG-INFO` & `variational-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: variational
-Version: 0.2.2
+Version: 0.3.0
 Summary: Variational Reference SDK
 Project-URL: Homepage, https://variational.io
 Project-URL: Documentation, https://docs.variational.io/for-developers/api
 Project-URL: Repository, https://github.com/variational-research/variational-sdk-python/
 Project-URL: Issues, https://github.com/variational-research/variational-sdk-python/issues
 Author-email: Variational Research <hello@variational.io>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Requires-Dist: brotli>=1.0
 Requires-Dist: requests>=2.12
 Description-Content-Type: text/markdown
 
 # Variational SDK for Python 
 
 ## Documentation
```

